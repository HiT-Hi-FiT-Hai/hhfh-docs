# Overview

All commands need to be **prefixed with one of these characters:**

- `+` (plus)
-`-` (subtract)
- `*` (caret),
- `/` (forward-slash)
- `!` (exclamation mark)
- `#` (hash)
- `?` (question mark). 

These commands are **sent as a private message** to **`[BOT]Info`**. 

If you think that this documentation is missing something
or it can be repharased/tweaked to make it more user-friendly, feel free to send in a pull request. 

**Note:** We have used **`/` (forward-slash)** as the prefix in this document, but you can use any of the above mentioned prefixes. 

**Important:** LinuxDC++ and some other clients do not support **`/` (forward-slash)** as a prefix, so, you must use any of the other prefixes mentioned above.

# Content
The commands are sub-divided into following categories:

1. Reading databases commands
1. Adding to tables
1. Deletion from tables
1. Miscellaneous commands

# Key
The following provides a short index of user-input variables referenced later in documentation.

    <#ID>          Number         An ID for respective tabular array
    <Lctg>         String         Valid categories as for latest entries
    <Bctg>         String         Categories applicable to buy and sell section; one of BUY, LOAN, SELL or HIRE
    <msg>          String         Complete string to be added

# Detailed guide on USAGE

> The content inside angular brackets represents user-input. If a
> user input is enclosed in square brackets, then it is optional and
> can be skipped by users.

## SECTION 1 - READING

 * `/readall [<#LIMIT>]` - generates a list of recent entries from all the tables. The number passed acts as a limit to this
     list and is default set to 10. **Shorthand** for the command is `rall`.

All the other read commands act in similar fashion and are listed as follows. The optional argument that can be passed is
again a non-negative number less than 50. Default value for limit is 15.

 * `/readreq [<#LIMIT>]` - lists recent requests. **Shorthand:** `rreq`
 * `/readbuysell [<#LIMIT>]` - lists recent buy and sell messages with possible replies on them.**Shorthand:** `rbsell`
 * `/readsug [<#LIMIT>]` - lists recent suggestions from users. **Shorthand:** `rsg`
 * `/readdels [<#LIMIT>]` - lists recent information from users about to delete something from their share. **Shorthand:** `rdel`
 * `/readgst [<#LIMIT>]` - lists recent guest book entries from users wanting to leave an impact on HiT Hi FiT Hai. **Shorthand:** `rgst`
 * `/readnws [<#LIMIT>]` - lists recent news items added by fellow users. **Shorthand:** `rn`

## SECTION 2 - ADDING

 * `/areq <Lctg> <msg>` - Adds your `<msg>` to respective `<Lctg>` and returns with an unique ID so that you might
     fill/delete it later. Please try to add a relevant link to whatever you are requesting. **Shorthand:** `ar <Lctg> <msg>`
 * `/asug <Lctg> <msg>` - This'll add your `<msg>` to the suggestions section. You should share a good tv series or a nice
     movie with others. **Shorthand:** `asg`
 * `/addbns <Bctg> <msg>` - Adds the `<msg>` to buy and sell table in database. Please also include your contact
     information. **Shorthand:** `absell`
 * `/addreply <msg>` - lets you add your messages/replies to content added in buy and sell section. Your reply must be preceded
     by a valid numerical ID from BnS. When you add a reply, the interested user gets notified. **Shorthand:** `amsg`
 * `/anws`, `/agst`, `/adel` all are independent segments and you can add to them without any restrictions. Just keep the
     messages shorter than 200 characters and don't use ALL CAPS.
     1. `/anws <msg>` - Add a news segment. **Shorthand:** `an`
     2. `/agst <msg>` - Enter your message in guestbook. Only one entry per user is allowed. So make it count. Oh, as a pre-warning
         you can NOT delete them. **Shorthand:** `ag`
     3. `/adel <msg>` - Inform users about something you are going to remove from your share so that others might
         mirror it while they have a chance. **Shorthand:** `ad`

## SECTION 3 - DELETING

All the deletion statements need a valid ID for respective tables. Other than that, you also *need to either have VIP+ powers* or
the **entry must have been added by you** to delete them.

 * `/delreq` - Deletes from request table. **Shorthand:** `dr`
 * `/delsug` - Remove a suggestion you might think is bloated. **Shorthand:** `dsg`
 * `/delnws` - Erase a news entry. **Shorthand:** `dn`
 * `/delbns` - To be used when you forgot to add some vital information in your message. **Shorthand:** `dbsell`
 * `/delmsg` - You might've wanted to add reply to some other message maybe. **Shorthand:** `dmsg`

## Section 4 - Others

 * `/help` - shows this help text.
 * `/fill <#ID>` - applicable only to unfilled requests; fills up the request marking it your nickname and informing
     the requester that you've done so.
 * `/switch <#ID>` - pertinent to buy and sell table so that you may mark your thread as old. This is useful for closing
     older deals. The command changes status of threads to *BOUGHT* or *SOLD* as applicable.
 * `/close <#ID>` - acts similar to `fill` but is usable by moderators and above power-users only. The requester is still
     notified about the action. It is used for ineffective or non-fillable requests.
