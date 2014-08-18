wp-cli-bh-shared
================

Use this to alias WP-CLI to 'wp' on a Bluehost shared hosting account (will work for Hostmonster and Just Host as well). Since WP-CLI is already on Bluehost's servers by default, this basically just creates the alias in your .bashrc file, sources it and makes it usable with running ```wp```, e.g. ```wp option get siteurl``` or ```wp user list```. For more information about WP-CLI, you can check it out here: [http://wp-cli.org/](http://wp-cli.org/) and you can find a list of commands to use with it here: [http://wp-cli.org/commands/](http://wp-cli.org/commands/).

The idea is to put this somewhere you can call on it (such as on your main server) and run it via curl on the hosting account you need it on (see "Usage" below).

Ideal for developers and web masters.

## Installation

### _Self Hosted (you host the file)__
Run the following from the directory on your server you would like to run this from:
```
git clone https://github.com/curtjen/wp-cli-bh-shared.git
```

### __Lazy Way (GitHub hosted)__
Refer to "Usage" instructions below (under "__Lazy Way (GitHub hosted)__").


## Usage

### __Self Hosted (you host the file)__
1. Connect via SSH to the hosting account that you would like to run this on.
2. Run the following command (note the dot "."):
```
. <(curl -sS PATH-TO-FILE)
```
3. Start using ```wp``` for running WP-CLI commands.

### __Lazy Way (GitHub hosted)__
1. Connect via SSH to the hosting account that you would like to run this on.
2. Run the following command (note the dot "."):
```
. <(curl -sS https://raw.githubusercontent.com/curtjen/wp-cli-bh-shared/master/wpcli)
```
3. Start using ```wp``` for running WP-CLI commands.
