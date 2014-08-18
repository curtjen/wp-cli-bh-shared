wp-cli-bh-shared
================

Use this to alias WP-CLI to 'wp' on a Bluehost shared hosting account. Ideal for developers or web masters. Since WP-CLI is already on Bluehost's servers by default, this basically just creates the alias in your .bashrc file and sources it. 

The idea is to put this somewhere you can store it (such as on your main server) and run it via curl on the hosting account you need it on.

## Installation

Run the following from the directory you would like to run this from.


## Usage

1. Connect via SSH to the hosting account that you would like to run it on.
2. Run the following command:
```
. <(curl -sS PATH-TO-FILE)
```
