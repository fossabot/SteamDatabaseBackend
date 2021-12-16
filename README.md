# Steam Database Backend
[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2FIanE-Official%2FSteamDatabaseBackend.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2FIanE-Official%2FSteamDatabaseBackend?ref=badge_shield)


The application that keeps [SteamDB](https://steamdb.info/) up to date with the latest changes directly from Steam,
additionally it runs an IRC bot and announces various Steam stuff in #steamdb and #steamdb-announce on [Freenode](https://freenode.net/).

This source code is provided as-is for reference. It is highly tuned for SteamDB's direct needs and is not a generic application.
If you plan on running this yourself, keep in mind that we won't provide support for it.

## Requirements
* [.NET Core](https://dot.net)
* [MySQL](https://www.mysql.com/) or [MariaDB](https://mariadb.org/) server

## Installation
1. Import `_database.sql` to your database
2. Copy `settings.json.default` to `settings.json`
3. Edit `settings.json` as needed: database connection string and Steam credentials.

Use `anonymous` as the Steam username if you need to debug quickly.

## IRC

We use [ZNC](http://znc.in) in front of our IRC bot to handle reconnections, staying in channels, flood protection and stuff like that.

There are some modules that are particularly useful to have:

* [keepnick](http://wiki.znc.in/Keepnick)
* [kickrejoin](http://wiki.znc.in/Kickrejoin)
* [stickychan](http://wiki.znc.in/Stickychan)
* [prioritysend](https://github.com/xPaw/znc-prioritysend) *(custom module)*

## License
Use of SteamDB Updater is governed by a BSD-style license that can be found in the LICENSE file.


[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2FIanE-Official%2FSteamDatabaseBackend.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2FIanE-Official%2FSteamDatabaseBackend?ref=badge_large)