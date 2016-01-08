# Overview

All commands need to be **prefixed with one of these characters:**

- `+` (plus)
- `-` (subtract)
- `*` (caret)
- `/` (forward-slash)
- `!` (exclamation mark)
- `#` (hash)
- `?` (question mark)

These commands are **sent as a private message** to **`[BOT]Stats`**. 

If you think that this documentation is missing something
or it can be repharased/tweaked to make it more user-friendly, feel free to send in a pull request. 

**Note:** We have used **`/` (forward-slash)** as the prefix in this document, but you can use any of the above mentioned prefixes. 

**Important:** LinuxDC++ and some other clients do not support **`/` (forward-slash)** as a prefix, so, you must use any of the other prefixes mentioned above.

# Contents
1. Chat Statisitcs  
	a. Open to all users  
	b. Open to registered users only
2. Toks
3. Polls

# Chat Statistics

### All Users

The following commands have been made available to all users:

-	`/top [<date>] [#Limit]` : Top chatterers of the day. Optional date argument can be passed
		in YYYY-MM-DD format. Argument #Limit is optional as well. Default limit is 10.
-	`/topall [#Limit]` : Top chatterers of all time. Argument #Limit is optional. Default limit is 10.

### Registered Users

The following commands are available for all users, but result will be produced only for
registered users. Unregistered users may either receive an error or undesired behaviour.

- `/see` : To get chat statistics for self.
-	`/score <nick>` : To fetch statistics of a registered user with nick as passed as arguments.


# Toks

Toks is recorded only for registered users.

- `/toks <nick>` - To fetch toks record of a registered user with nick as passed as
	arguments. Nick is optional, if not passed default value would be your nick.
- `/rich [#limit]` - Users with highest toks currently. Argument #Limit is optional. If
	not passed, default value would be 15.
-	`/richest [#limit]` - Users with highest toks over all time. Argument #Limit is
	optional. If not passed, default value would be 15.
- `/gift <nick> <#amount> <message>` - To gift specified amount of toks to registered
	user with the given nick. Message is optional.

# Polls

While any user can participate in an ongoing poll, only registered users are allowed to
create new ones. The following commands are available to the end users:

- `/poll add <msg>` - To add a new poll to the database. The format for providing list of choices is as follows:

            /poll add Is this feature awesome?[]Yes [] No[]Maybe

        **NOTE:** Spaces around the `[]` delimiters will be ignored.

- `/poll remove <#ID>` - Provide a valid ID for a poll to delete it.
- `/poll view <#ID>` - Detailed voting break-down for the poll with provided ID will be returned.
- `/poll list [<#Limit>]` - Default limit is 15. only the most recent #Limit polls will be displayed.
- `/poll vote <#Poll> <#Choice>` - Cast your vote for the #Choice of the poll with ID #Poll.
- `/poll help` - Display help selectively for the polling features.
