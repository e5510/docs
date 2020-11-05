# Commands for Everyone
Everyone have access to these commands.

- [c!count](#ccount): Get the current count.
- [c!help](#chelp): Get help on how to use the bot.
- [c!info](#cinfo): Get information and stats about the bot.
- [c!notifications](#cnotifications): Get a list of your notifications in the server.
- [c!notifyme](#cnotifyme): Get a notification whenever the server reach whatever count you want.
- [c!ping](#cping): Get the latency of the bot.
- [c!removenotif](#cremovenotif): Remove a notification.
- [c!scoreboard](#cscoreboard): Get the current scoreboard of the server.

# Commands for Mods
Everyone with the Manage Messages-permission have access to these commands.

- [c!listflows](#clistflows): Get a list of all the flows.
- [c!listregex](#clistregex): Get a list of regex filters.
- [c!setcount](#csetcount): Set the count.

# Commands for Admins
Everyone with the Manage Server-permission have access to these commands.

- [c!addregex](#caddregex): Add a regex filter. (useful with the talking module)
- [c!addtoscore](#caddtoscore): Add to a member's score (or multiple members' scores)
- [c!createflow](#ccreateflow): Create a new flow to customize your counting setup completely.
- [c!deleteflow](#cdeleteflow): Delete a flow.
- [c!disabletimeoutrole](#cdisabletimeoutrole): Reset and disable the timeout role.
- [c!editflow](#ceditflow): Edit a flow.
- [c!exportscores](#cexportscores): Export scores to a JSON-file.
- [c!importscores](#cimportscores): Import scores from a JSON-file. Upload the JSON-file with the command itself.
- [c!link](#clink): Link a counting channel manually.
- [c!module](#cmodule): Manage modules you can enable or disable in your server.
- [c!prunescores](#cprunescores): Prune the scoreboard for members who have left your server.
- [c!removefromscore](#cremovefromscore): Set a member's score
- [c!removeregex](#cremoveregex): Remove a regex filter.
- [c!resetcount](#cresetcount): Reset the count.
- [c!resetscore](#cresetscore): Reset a member's score (or multiple members' scores)
- [c!setprefix](#csetprefix): Set the prefix of the bot.
- [c!setscore](#csetscore): Set a member's score (or multiple members' scores)
- [c!settimeoutrole](#csettimeoutrole): Set a member's score (or multiple members' scores)
- [c!setup](#csetup): Quickly set up a counting channel. You only need to do this once.
- [c!unlink](#cunlink): Unlink the current counting channel.

# Commands for Server Owners
Only the server owner has access to these commands.

- [c!dump](#cdump): Dump a server's data to DMs. (GDPR-compliant)
- [c!factoryreset](#cfactoryreset): Reset all data Countr has stored about this server.

## c!addregex

Add a regex filter. (useful with the talking module)

**Usage:** `c!addregex <regex ...>`
- `<regex ...>`: The regex you want to filter out of the chat. Get info on how to create a regex here: https://flaviocopes.com/javascript-regular-expressions/#regular-expressions-choices

**Examples:**
- `c!addregex duck|poop`: Will filter out all messages containing duck and/or poop.
- `c!addregex [A-Z]`: Will filter out all messages with capital letters.
- `c!addregex [A-Ca-cX-Zx-z]`: Will filter out A, B, C, X, Y, Z - regardless if it's capital or not.

**Permission Level:** 2, Admins

**Aliases:** `+regex`, `addfilter`, `+filter`

## c!addtoscore

Add to a member's score (or multiple members' scores)

**Usage:** `c!addtoscore <member(s ...)> <number>`
- `<member(s ...)>`: The member(s) you want to add the score of
- `<number>`: The number you want to add to the scores

**Examples:**
- `c!addtoscore 110090225929191424 9999999`: Add 9999999 to user with ID 110090225929191424.
- `c!addtoscore @Promise#0001 1337`: Add 1337 to Promise#0001's score.
- `c!addtoscore 110090225929191424 @Promise#0001 1000`: Add 1000 to user with ID 110090225929191424 and to Promise#0001.

**Permission Level:** 2, Admins

**Aliases:** `+score`

## c!count

Get the current count.

**Permission Level:** 0, All

**Aliases:** `!`

## c!createflow

Create a new flow to customize your counting setup completely.

**Permission Level:** 2, Admins

**Aliases:** `addflow`, `+flow`

## c!deleteflow

Delete a flow.

**Usage:** `c!deleteflow <flow ID>`
- `<flow ID>`: The ID of the flow you want to delete. This can be found in the 'listflows'-command.

**Permission Level:** 2, Admins

**Aliases:** `delflow`, `removeflow`, `-flow`

## c!disabletimeoutrole

Reset and disable the timeout role.

**Permission Level:** 2, Admins

**Aliases:** `resettimeoutrole`, `re=timeoutrole`

## c!dump

Dump a server's data to DMs. (GDPR-compliant)

**Permission Level:** 3, Server Owner

**Aliases:** `export`

## c!editflow

Edit a flow.

**Usage:** `c!editflow <flow ID>`
- `<flow ID>`: The ID of the flow you want to edit. This can be found in the 'listflows'-command.

**Permission Level:** 2, Admins

**Aliases:** `modifyflow`, `=flow`

## c!exportscores

Export scores to a JSON-file.

**Usage:** `c!exportscores <member(s ...)>|raw`
- `<member(s ...)>|raw`: The member(s) you want to export the scores of.

**Examples:**
- `c!exportscores 110090225929191424`: Export the score of user with ID 110090225929191424.
- `c!exportscores @Promise#0001`: Export the score of user Promise#0001.
- `c!exportscores 110090225929191424 @Promise#0001`: Export the scores of user with ID 110090225929191424 and user Promise#0001.
- `c!exportscores raw`: Export all scores raw.

**Permission Level:** 2, Admins

## c!factoryreset

Reset all data Countr has stored about this server.

**Permission Level:** 3, Server Owner

## c!help

Get help on how to use the bot.

**Usage:** `c!help [search ...]`
- `[search ...]`: Something you want to search for, for example a command.

**Examples:**
- `c!help help`: Get help on the command help. Oh wait, you already did.

**Permission Level:** 0, All

**Aliases:** `commands`

## c!importscores

Import scores from a JSON-file. Upload the JSON-file with the command itself.

**Usage:** `c!importscores set|add`
- `set|add`: Decide if you want to overwrite the scores or add to the existing scores.

**Examples:**
- `c!importscores set`: Will overwrite all the scores to the one in the file.
- `c!importscores add`: Will add the scores to the users' previous scores.

**Permission Level:** 2, Admins

## c!info

Get information and stats about the bot.

**Permission Level:** 0, All

**Aliases:** `stats`, `botinfo`, `botstats`

## c!link

Link a counting channel manually.

**Usage:** `c!link [<channel>]`
- `[<channel>]`: The new counting channel. Leave empty to choose current channel.

**Permission Level:** 2, Admins

**Aliases:** `connect`

## c!listflows

Get a list of all the flows.

**Permission Level:** 1, Mods

**Aliases:** `flows`

## c!listregex

Get a list of regex filters.

**Permission Level:** 1, Mods

**Aliases:** `regexlist`, `regexfilters`, `listfilters`

## c!module

Manage modules you can enable or disable in your server.

**Usage:** `c!module [<module>] [on|off]`
- `[<module>]`: The module you want more information on, or turn on/off.
- `[on|off]`: Whether you want to turn the module on or off.

**Examples:**
- `c!module allow-spam on`: Toggle the module allow-spam.
- `c!module webhook`: Get more help on the webhook-module.

**Permission Level:** 2, Admins

**Aliases:** `modules`

## c!notifications

Get a list of your notifications in the server.

**Permission Level:** 0, All

**Aliases:** `notiflist`, `notifs`, `alerts`, `listalerts`, `listnotifs`, `listnotifications`

## c!notifyme

Get a notification whenever the server reach whatever count you want.

**Usage:** `c!notifyme [each] <count>`
- `[each]`: If you include this, it will notify you of a multiplication of &lt;count&gt;.
- `<count>`: The count you want to get notified of.

**Examples:**
- `c!notifyme 420`: Get notified whenever the server reach count 420.
- `c!notifyme each 1000`: Get notified for every 1000th count, including 2000 and 3000 and so on.

**Permission Level:** 0, All

**Aliases:** `alertme`, `notify`, `alert`

## c!ping

Get the latency of the bot.

**Permission Level:** 0, All

**Aliases:** `pong`, `latency`, `uptime`

## c!prunescores

Prune the scoreboard for members who have left your server.

**Permission Level:** 2, Admins

## c!removefromscore

Set a member's score

**Usage:** `c!removefromscore <member(s ...)> <score>`
- `<member(s ...)>`: The member(s) or members of role(s) you want to set the score of
- `<score>`: The new score

**Examples:**
- `c!removefromscore 110090225929191424 9999999`: Will set member with ID 110090225929191424's score to 9999999.
- `c!removefromscore @Promise#0001 @CountingGods 1337`: Will set Promise#0001's and all members in role Counting Gods' score to 1337.

**Permission Level:** 2, Admins

**Aliases:** `-fromscore`, `-score`

## c!removenotif

Remove a notification.

**Usage:** `c!removenotif <ID(s ...)>|all`
- `<ID(s ...)>|all`: The notification ID(s) you want to remove, or all notifications.

**Examples:**
- `c!removenotif bd9kJK`: Remove notification with ID bd9kJK.
- `c!removenotif all`: Remove all notifications.

**Permission Level:** 0, All

**Aliases:** `-notif`

## c!removeregex

Remove a regex filter.

**Usage:** `c!removeregex <regex ...>`
- `<regex ...>`: The regex filter you want to remove.

**Examples:**
- `c!removeregex duck|poop`: Will remove the regex filter `duck|poop`.

**Permission Level:** 2, Admins

**Aliases:** `-regex`, `removefilter`, `-filter`

## c!resetcount

Reset the count.

**Permission Level:** 2, Admins

**Aliases:** `re=count`, `reset`

## c!resetscore

Reset a member's score (or multiple members' scores)

**Usage:** `c!resetscore <member(s ...)>|all`
- `<member(s ...)>|all`: The member(s) you want to add the score of, or all.

**Examples:**
- `c!resetscore 110090225929191424`: Reset score of user with ID 110090225929191424.
- `c!resetscore @Promise#0001`: Reset score of Promise#0001.
- `c!resetscore 110090225929191424 @Promise#0001`: Reset score of user with ID 110090225929191424 and Promise#0001.
- `c!resetscore all`: Reset all scores.

**Permission Level:** 2, Admins

**Aliases:** `re=score`

## c!scoreboard

Get the current scoreboard of the server.

**Permission Level:** 0, All

**Aliases:** `leaderboard`, `^`, `top`

## c!setcount

Set the count.

**Usage:** `c!setcount <count>`
- `<count>`: The new count.

**Permission Level:** 1, Mods

**Aliases:** `set`, `=`, `=count`

## c!setprefix

Set the prefix of the bot.

**Usage:** `c!setprefix [prefix ...]`
- `[prefix ...]`: The new prefix you'd like to use. Leave blank to reset.

**Examples:**
- `c!setprefix c?`: Set the prefix to `c?`.

**Permission Level:** 2, Admins

**Aliases:** `prefix`

## c!setscore

Set a member's score (or multiple members' scores)

**Usage:** `c!setscore <member(s ...)> <score>`
- `<member(s ...)>`: The member(s) or members of role(s) you want to set the score of
- `<score>`: The new score

**Examples:**
- `c!setscore 110090225929191424 9999999`: Set score to 9999999 for user with ID 110090225929191424.
- `c!setscore @Promise#0001 1337`: Set score to 1337 for Promise#0001's score.
- `c!setscore 110090225929191424 @Promise#0001 1000`: Set score to 1000 for user with ID 110090225929191424 and for Promise#0001.

**Permission Level:** 2, Admins

**Aliases:** `=score`

## c!settimeoutrole

Set a member's score (or multiple members' scores)

**Usage:** `c!settimeoutrole <role> <fails> <time> [<duration>]`
- `<role>`: The role you want the timeout role to be. If you plan on using the role name, surround it with quotation marks.
- `<fails>`: The amount of fails within &lt;time&gt; seconds to get the role.
- `<time>`: Time in seconds users have to count &lt;fails&gt; times to get the role.
- `[<duration>]`: Duration in seconds the role will stay on for. Without a value, it will stay on the user forever.

**Examples:**
- `c!settimeoutrole "Timed out" 5 10`: This will give the user the role Timed out if they fail 5 times within 10 seconds.
- `c!settimeoutrole @Timeout 3 30 120`: This will give the user the role Timeout if they fail 3 times within 30 seconds, and the role will be removed after 2 minutes.

**Permission Level:** 2, Admins

**Aliases:** `=timeoutrole`

## c!setup

Quickly set up a counting channel. You only need to do this once.

**Permission Level:** 2, Admins

**Aliases:** `autosetup`, `quicksetup`, `configure`

## c!unlink

Unlink the current counting channel.

**Permission Level:** 2, Admins

**Aliases:** `disconnect`