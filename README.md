Pandaren5.3.0
=============

World of Warcraft Mists of Pandaria emulator for 5.3.0 (17128)

READ ME :

PATCHED CLIENT(x86)Windows - http://www.sendspace.com/file/qwrgly	
DBC - http://www.sendspace.com/file/9euiv9	
MAPS - http://www.sendspace.com/file/5miivl	


TO DO:
Fix "self" UPDATE_OBJECT for player. That's the problem why full login doesn't work.

For those who fork it.
1. There are 2 updates for "auth" that needs to be executed (don't forget about them).
2. I hope people will push something not only pull and wait for other.






= TrinityCore -- General information =

Copyright (C) TrinityCore (http://www.trinitycore.org)

  Trinity Core is free software; you can redistribute it and/or modify
  it under the terms of the GNU General Public License as published by
  the Free Software Foundation; either version 2 of the License, or
  (at your option) any later version.

  This program is distributed in the hope that it will be useful,
  but WITHOUT ANY WARRANTY; without even the implied warranty of
  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  GNU General Public License for more details.

  You should have received a copy of the GNU General Public License
  along with this program; if not, write to the Free Software
  Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA

  In addition, as a special exception, the Trinity Core project
  gives permission to link the code of its release of Trinity Core with
  the OpenSSL project's "OpenSSL" library (or with modified versions of
  it that use the same license as the "OpenSSL" library), and distribute
  the linked executables.  You must obey the GNU General Public License
  in all respects for all of the code used other than "OpenSSL".  If you
  modify this file, you may extend this exception to your version of the
  file, but you are not obligated to do so.  If you do not wish to do
  so, delete this exception statement from your version.

TrinityCore is a MMORPG Framework based mostly on C++. It is completely 
open source, and is community supported. It is derived
from MaNGOS, the Massive Network Game Object Server, and is based on the
code of that project with extensive changes over time to optimize, improve
and cleanup the codebase at the same time as improving the ingame mechanics
and functionality. If you wish to contribute ideas or code please visit 
our site linked below or make pull requests to our github repo at 
https://github.com/TrinityCore/TrinityCore

For further information on the TrinityCore project, please visit our
project website at http://www.TrinityCore.org

Documentation including installation instructions can be found inside
the doc directory.

SQL files to create the databases can be found in the sql/create and 
sql/base directories.
You need to run sql/create/create_mysql.sql 1st and then
sql/base/auth_database.sql and sql/base/characters_database.sql
You need to download world database from http://www.trinitycore.org/f/files/
be sure you get the higher numbered database.
When installing a core the 1st time you need to import also all the files at
sql/updates/world directory.
sql/updates/auth and sql/updates/characters databases only needs to be run
when updating one existing server.
To save time importing multiple files, you can use copy *.sql world_updates.sql
under Windows or cat *.sql > world_updates under Linux.

You need to update your core (recompile and overwrite binaries) when updating
your database, usually you can't use one older core with a newer database or a
newer core with an older database.
When updating your core you also need to import the files at sql/updates/auth
and sql/updates/characters along with the sql/updates/world files.
You can't merge all the sql files on sql/updates into a single file, because
they belong to 3 different databases and they don't use database name.

TrinityCore Requirements
Platform: Linux, Windows or Mac
Processor with SSE2 support
ACE ≥ 5.8.3
MySQL ≥ 5.1.0
CMake ≥ 2.8.0
OpenSSL ≥ 0.9.8o
GCC ≥ 4.3 (Linux only)
MS Visual Studio ≥ 9 (2008) (Windows only)
A bit of brain, wiki can become outdated with the release of new TDB versions
if wiki refers to TDB 50 and you see TDB 52 get the higher number.
Some reading skills, search forum, read http://www.trinitycore.org/f/topic/1518-
and http://www.trinitycore.org/f/topic/37- before posting a bug report or ask for
help on forum. 
Search for existing bug reports before posting your own bug reports; don't post multiple
bugs on a single ticket.
