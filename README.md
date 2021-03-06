# Buttercup Archive Importer
Import archives from other password managers.

[![npm version](https://badge.fury.io/js/buttercup-importer.svg)](https://github.com/buttercup/buttercup-importer) [![minium node version](https://img.shields.io/badge/node%20version-%3E%3D%206.x-blue.svg)](https://github.com/buttercup/buttercup-importer) [![Build Status](https://travis-ci.org/buttercup/buttercup-importer.svg?branch=master)](https://travis-ci.org/buttercup/buttercup-importer)

## About
This archive importer coverts password archives from other formats to the Buttercup archive format (BCUP).

### Supported platforms
The importer requires Node **6** or higher.

### Supported password archive formats

* ![KDBX (keepass)](https://img.shields.io/badge/KDBX-Full-brightgreen.svg) KeePass 2 archives
* ![Lastpass](https://img.shields.io/badge/CSV-Full-brightgreen.svg) Lastpass archives
* ![1Password](https://img.shields.io/badge/1PIF-Basic-brightgreen.svg) 1Password PIF files (exported)
* ![CSV](https://img.shields.io/badge/CSV-None-red.svg) CSV files (general)

### Importing from 3rd-party managers

#### KeePass 2
KeePass archives for KeePass 2 can be opened using the `importFromKDBX` command. Simply pass the filename, password and destination path.

#### 1Password
When your archive is open, choose to export all entries to 1PIF format. Provide the path and destination to the `importFrom1PIF` function.

Imported 1Password archives may lose some information regarding their type (eg. Credit cards).

#### LastPass
Lastpass credentials can be exported as CSV files, which can be imported using Buttercup importer.
