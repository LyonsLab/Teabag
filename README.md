Teabag - CoGe's Utility Belt
============================

Teabag is a bash script that manages CoGe services abstracting away the need for multiple, messy CLI calls.

## Dependencies ##

Teabag has a few dependencies for operation and formatting that might not come
default on most unix systems. They are:

* pgrep - a process grep program
* pkill - a process killer program

## Installation ##
Teabag comes pre-installed on the coge dev server, but if you don't have access to this fine machine never fear:

1. `mv <the teabag script> /usr/local/bin/teabag`
2. `sudo chmod 755 teabag`

## Configuration ##

Configuring Teabag to work on your system is as simple as changing some config
variables in the script.

Open the teabag script in your favorite text editor and change these
configuration settings located at the top of the file:

    ##################################
    #     Configuration Settings     #
    ##################################
    GREENTEA_DIR='&lt;Greentea's Root Path&gt;'
    GREENTEA_LOG_FILE='$GREENTEA_DIR/logs/error.log'
    URL='geco.iplantc.org/analytics'
    FONT='invita'

## Usage ##

To __start__ up all the currently configured processes:

* `teabag`

To __start specific__ processes:

* `teabag infuse <process>`

To __check__ which __processes__ Teabag is currently configured for:

* `teabag processes`

To __check__ the __status__ of all currently configured proccesses:

* `teabag status`

To __kill__ all running processes:

* `teabag kill`

To __kill specific__ processes:

* `teabag kill <process>`

To list all usable __commands__:

* `teabag usage`

To restart the __apache__ server alone:

* `teabag apache`

For __help__ with any commands:

* `teabag help <command>`
