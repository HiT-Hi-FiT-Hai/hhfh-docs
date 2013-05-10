The commands are divided into following sub-sections:

 - For all users:
    1. latest or l
    2. search or s
    3. msg or m
    3. showctg or sc
    4. showmods or sm
    5. help or h
    6. rules or r
 - For moderators and above:
    1. addlatest or al
    2. dellatest or dl
    3. updatelatest or ul
    4. addmagnet or am
    6. editmagnet or em
    7. removemagnet or rm
 - For VIP and above
    1. addmod
    2. delmod
 - For Operators and key users
    1. addctg
    2. delctg

# Detailed guide on USAGE

## FOR ALL USERS

+latest (or simply +l) can be used in one of the following ways:

01. +l
	This will just list the newest 35 entries from the latest database sorted by the date. You can supply a number greater than 5
	  and smaller than 35 to limit result to those many entries.

02. +l <ctg>
	Any of the categories can be given as argument. You'll get a default 20 entries if the category exists otherwise works same as
	  +latest. An additional limit number can be provided.

+search (or +s) must be given with a search string of length greater than 3 characters.

+showctg (or +sc) lists all the available categories. Helpful for both new moderators and users.

+showmods (or +sm) lists all current moderators on the hub.

+rules ( or +r ) populatest the general rules for entries.

+help ( or +h ) shows this help.


## FOR MODERATORS

+addlatest( or +al ) must be followed with a category, entry string and magnet in that order. A descriptive rules for formatting
    and other details are explained under rules. General rules can be accessed using +rules( or +rules )

+updatelatest( or +ul ) should be followed by the entry ID and new string. If the entry was not made by you, you can not update it.

+dellatest( or +dl ) accepts only a single numerical argument, the entry ID from latest entries. Deleted the row from table.

+addmagnet( or +am ) requires 2 arguments. The addition entry ID and the magnet to be added. The ID must be a valid entry from
    the table. Non-numerical values are no accepted.

+editmagnet( or +em ) does the same task as `+em` except only for magnet ID. They are shown with the respective magnet in latest
    table display.

+removemagnet( or +rm ) must be passed with a valid numerical magnet ID. It removes the magnet associated with that ID.


## FOR VIPs & ABOVE USERS

In addition to all the commands above, following commands have also been made available to you:

+addmod requires one argument, being the nickname of a registered user on hub. It adds the user to moderators list, so that they
    can also add entries to latest database.

+delmod just deletes the user(nick passed as argument) from moderator privileges.
