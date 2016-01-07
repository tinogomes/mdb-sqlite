# mdb-sqlite
Automatically exported from [code.google.com/p/mdb-sqlite](http://code.google.com/p/mdb-sqlite)

## Description
Provides automated conversion of [MS Access 2000](https://en.wikipedia.org/wiki/Microsoft_Access) databases to [SQLite](https://www.sqlite.org/) on any platform, utilizing [Jackcess](http://jackcess.sourceforge.net/) and [SQLite Java libraries](http://www.zentus.com/sqlitejdbc/). No native driver required.

MDB-SQLite is used by [Plausible Labs](http://www.plausiblelabs.com/) to read government-supplied Access databases.

## Usage
To compile, run:

`$ ant dist`

This will create a standalone jar in `dist/mdb-sqlite.jar`

To convert a database file:

`$ java -jar dist/mdb-sqlite.jar source.mdb output.sqlite`

## Changes
1.0.2 Release
- Prefix index names with the table names to prevent name conflicts when converting indixes.

1.0.1 Release
- Work-around around the SQLite JDBC drivers lack of support for boolean values

- Add support for converting indexes

1.0 Release
- Initial Release
