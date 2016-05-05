[![build status](http://betahoster.com:773/jarrrk/DBSync/badges/master/build.svg)](http://betahoster.com:773/jarrrk/DBSync/builds)

### What is DBSync?
DBSync is a Linux command-line utility allowing for easy database changes between application versions. It was originally built in-house for [GoGreen's](http://gogreen.co.uk) internal build platform but later realized a wider audience may also find this tool useful.

### Usage
Integrating DBSync into a project takes just a few minutes. Start by downloading the latest release found [here](http://betahoster.com:773/Jarrrk/DBSync/tags), inside the archive you will find a example folder, inside will be two files; copy these two files in to the directory of your project and edit `dbs_config.json` to match your database settings. Once finished you can now start adding your SQL statements in to the `dbs_updates.json` file.

DBSync is a bare-minimum executable, meaning there aren't any command-line arguments (yet). Run the command `dbsync` in any directory where there is a valid `dbs_config.json` & `dbs_updates.json`

Something not working quite right? You can enable verbose outputting by setting an environmental variable like so: `export DBSYNC_DEBUG=true`

### Requirements
* JDK/JRE 1.6 or upwards
* Sufficient database user permissions (CREATE, SELECT, UPDATE, INSERT)

### Install Instructions
Simply download the latest release and copy the `bin/dbsync` file from the downloaded archive in to your `/usr/bin/` system folder.

After you've moved the file you will want to make it executable using: `chmod +x /usr/bin/dbsync`

That's pretty much it, see usage instructions.

### Credits
* Initial Design - David Hinchliffe & Jack Carlin
* Programming - Jack Carlin

### License
Copyright 2016 Jack Carlin

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
