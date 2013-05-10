# Contents
The commands are divided into following sub-sections:

 - For all users:
    1. latest or l
    1. search or s
    1. msg or m
    1. showctg or sc
    1. showmods or sm
    1. help or h
    1. rules or r
 - For moderators and above:
    1. addlatest or al
    1. dellatest or dl
    1. updatelatest or ul
    1. addmagnet or am
    1. editmagnet or em
    1. removemagnet or rm
 - For VIP and above
    1. addmod
    1. delmod
 - For Operators and key users
    1. addctg
    1. delctg

# Detailed guide on USAGE

> The content inside angular brackets represents user-input. All
> commands need to be prefixed with one of these characters:
> **`+`**(plus), **`-`**(subtract), **`*`**(caret), **`/`**(forward-slash), **`!`**(exclamation mark),
> **`#`**(hash), **`?`**(question mark).

## FOR ALL USERS

 - `latest` can be used in one of the following ways:

    1. `l` - This will just list the newest 35 entries from the latest database sorted by the date. You can
    supply a number greater than 5 and smaller than 35 to limit result to those many entries.

    2. `l <ctg>` - Any of the categories can be given as argument. You'll get a default 20 entries if the
    category exists otherwise works same as `latest`. An additional limit number can be provided.

 - `search <string>` - The search string must have length greater than 3 characters.

 - `showctg` lists all the available categories. Helpful for both new moderators and users.

 - `showmods` lists all current moderators on the hub.

 - `rules` populatest the general rules for entries.

 - `help` shows this help.

## FOR MODERATORS

 - `addlatest <ctg> <entry> <magnetLink>` - A descriptive rules for formatting and other details are explained
 under rules. General rules can be accessed using **`+rules`**( or `+r` ).

 - `addmagnet <#EID> <magnetLink>` - The addition entry ID and the magnet to be added. The ID must be a
 valid entry from the table. Non-numerical values are no accepted.

 - `updatelatest <#EID> <newEntry>` - Update your previous entry while still keeping it in the same
 category. If the entry was not made by you, you can not update it; unless you have permissions.

 - `editmagnet <#MID> <newMagnetLink>` - Updates magnet related to certain magnet ID. They are shown with
 the respective magnet in latest table display.

 - `dellatest <#EID>` - The entry ID must be from latest entries. Deletes the row from table, if it exists
 otherwise returns error.

 - `removemagnet` - It removes the magnet associated with an ID.

## FOR VIPs
VIPs have the ability to add and remove moderators along with all commands listed above.

 - `addmod <nick>` - The user must be registered on the hub. It adds the user with nickname `<nick>` to
 moderators list, so that they can also add entries to latest database.

 - `delmod <nick>` - Deletes the user from moderator privileges.

## FOR Operators
In addition to all the commands above, following commands have also been made available to you:

 - `addctg <ctg>` - Add the category to list so that newer entries can be added to this category.

 - `delctg <ctg>` - Deletes the category from list.
