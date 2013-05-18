# Overview
All commands need to be prefixed with one of these characters: `+` (plus), `-` (subtract), `*` (caret),
`/` (forward-slash), `!` (exclamation mark), `#` (hash), `?` (question mark). These commands are sent
as a private message to **`[BOT]Info`**. If you think that this documentation is missing something
or it can rewritten/tweaked in a more user-friendly manner, feel free to send in a pull request.

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
    <Bctg>         String         Categories applicable to buy and sell section
    <msg>          String         Complete string to be added

# Detailed guide on USAGE

> The content inside angular brackets represents user-input. If a
> user input is enclosed in square brackets, then it is optional and
> can be skipped by users.

## SECTION 1 - READING

 * `readall` (or `rall`) followed by ONLY a non-negative numerical value below 35. It'll generate a list of recent entries from
    all the tables. The number passed acts as a limit to this list and is default set to 10.

All the other read commands act in similar fashion and are listed as follows. The optional argument that can be passed is
again a non-negative number less than 50. Default value for limit is 15.

 * `readreq` (or `rreq`) lists recent requests
 * `readbuysell` (or `rbsell`) lists recent buy and sell messages with possible replies on them
 * `readsug` (or `rsg`) lists recent suggestions from users
 * `readdels` (or `rdel`) lists recent information from users about to delete something from their share
 * `readgst` (or `rgst`) lists recent guest book entries from users wanting to leave an impact on HiT Hi FiT Hai
 * `readnws` (or `rn`) lists recent news items added by fellow users

## SECTION 2 - ADDING

 * `areq` (or `ar`) and `asug` (or `asg`) are similar commands and need to be followed first by one of the categories
     and then the actual message. If you are adding a request, please try to add a relevant link to whatever you are requesting.
 * `addbns` (or `absell`) succeeded by one of BUY, LOAN, SELL or HIRE and the object adds them to buy and sell table in
     database. Please also include your contact information.
 * `addreply` (or `amsg`) lets you add your messages/replies to content added in buy and sell section. Your reply must be preceded
     by a valid numerical ID from BnS. When you add a reply, the interested user gets notified.
 * `anws` (or `an`), `agst` (or `ag`), `adel` (or `ad`) all are independent segments and you can add to them without any
     restrictions. Just keep messages shorter than 200 characters and don't use ALL CAPS.

     1. `anws` - Add a news segment.
     2. `agst` - Enter your message in guestbook. Only one entry per user is allowed. So make it count. Oh, as a pre-warning
         you can NOT delete them.
     3. `adel` - Inform users about something you are going to remove from your share so that others might
         mirror it while they have a chance.

## SECTION 3 - DELETING

All the deletion statements need a valid ID for respective tables. Other than that, you also need to either have VIP+ powers or
the entry must have been added by you to delete them.

 * `delreq` (or `dr`) - Deletes from request table
 * `delsug` (or `dsg`) - Remove a suggestion you might think is bloated
 * `delnws` (or `dn`) - Erase a news entry
 * `delbns` (or `dbsell`) - To be used when you forgot to add some vital information in your message
 * `delmsg` (or `dmsg`) - You might've wanted to add reply to some other message maybe

## Section 4 - Others

 * `help` (or `h`) shows this help text.
 * `fill` followed by mandatory ID from a valid unfilled request; fills up the request marking it your nickname
     while informing the requester that you've done so.
 * `switch` accepts a numerical and valid ID from buy and sell section so that you may mark your thread as old. This is
     useful for closing older deals. The command changes status of threads to *BOUGHT* or *SOLD* as applicable.
 * `close` acts similar to `fill` but is usable by moderators and above power-users only. The requester is still
     notified about the action.

Please inform hjpotter92 in case of any problems you face related to newer Infobot
