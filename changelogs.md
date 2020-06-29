---
description: All changelogs for the bot will be posted here
---

# Changelogs

## v1.1.3

### Added

* Added our own API for the discord accounts bound to the Roblox account like `eryn.io` and `roverify`
* Added our own GUI and API for logging events in-game \(Which will be for partners only at the moment \) 

### Changed

* `Changelogs` command has been replaced with a link to the changelogs in the docs
* Changed the bot status check to a better one for more consistency  

### Fixed

* Fixed wrong API redirection

## v1.1.2

### Added

* Added snipe command for all of you snipers 😉 
* Added [Promote](commands/regiment/promoting-one-rank-higher.md) and [Demote](commands/regiment/demoting-one-rank-below.md) commands for servers set as regiments

### Changed

* Ranking in regiments and armies is now case-insensitive
* Revamped the `ping` command
* Disabled the `warnings` command as it has some bugs for now

### Fixed

* Fixed some common bugs and errors
* Fixed verification not working if the found id is banned



## v1.1.1

### Changed

* [Shout](commands/shout.md) command now shows the name of the person who used it in the shout

## v1.1.0 🎉 

Thank you all for the support and for reaching our first milestone **`50 servers`**

### Added

* New bot framework released with tons of new changes
* Better error logging
* Custom channels 
  * You can subscribe to our changelogs by making a channel called `soldier-updates`
  *  To get all bot log you can create a channel called `soldier-logs`

### Changed

* The [Setup](setup.md) has been revamped
* No more `ranking access` and `rank requesting` roles, you can now set up your own roles that will have ranking access and rank requesting permissions
* Custom channels too
* Stylish design for accepting requests for army ranking now
* Moved to a better host

### Fixed

* Fixed a bug where some servers can bind your groups to their servers while the group is already bound to your server

### Removed

* The guilds table in the database has been dropped so that new servers will have to set up their servers again to access the new changes
* `servercheck` command has been removed as it's needed anymore

## v1.0.9

### Changed

Switched verification APIs

## v1.0.8

### Added

* Added [Verify](commands/verify.md) command for user verification

{% hint style="info" %}
Start verifying your Roblox accounts to bind them to your discord for future uses
{% endhint %}

### Changed

* The bot status is now dynamic which changes every 6 seconds

## v1.0.7

### Added

* Bot checking in the group for all army/regiment commands
* Bot permissions check for discord added for all commands
* Bot permissions check for the group added for all army/regiment commands
* Channel checks for `servercheck` command has been added

### Changed

* The Ticket system is now `react for a ticket` way
* Maximum rank has been replaced by a dynamic check for ranking in armies and regiments

### Removed

* Maximum rank has been removed
* The `Ticket` command has been removed



## v1.0.6

### Added

* Added [Shout](commands/shout.md) command for both army and regiment server types
* Added [Welcomer](commands/welcomer.md) command for all server types so that you can set up a welcome/leave logs for your server and manage it through it 

## v1.0.5

### Changed

* Migrated to a better database host

### Fixed

* Fixed the bug where some times the bot was lacking permissions in his required channels

## v1.0.4

### Added

* Added `upvote` command so you can support us by voting for the bot on different discord bots lists
* Added `servercheck` command to check your server for the essential stuff required to run the bot perfectly.

### Changed

* Changed the default prefix to `s!`

{% hint style="info" %}
If your server is set up then your prefix is not changed
{% endhint %}

## v1.0.3

### Added

* Added more moderation commands `Warn` and `warnings`
* Moderation setup for users 

### Changed

* Changed the users who can setup/re-setup your server to people with administrator permissions in your server only
* You don't need to do `/invite bot` or `/invite support` anymore just doing `/invite`will send you both the invite link and the support server link

### Fixed

* Fixed the ticket duplications

## v1.0.2

### Added

* Added more moderation commands `Mute` and `Unmute`
* Suggestion approval and disapproval
* Better error reporting

### Changed

* The help command is dynamic which means it's will show commands that are executable by the user who called help



## V1.0.1

### Added

* Support server only commands
* Moderation commands \(Kick, Ban\)

## v1.0.0

**`Bot launch`**

