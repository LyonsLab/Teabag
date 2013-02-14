Teabag - CoGe's Utility Belt
============================

Teabag is a bash script that manages CoGe services abstracting away the need for multiple, messy CLI calls.

## Installation ##
Teabag comes pre-installed on the coge dev server, but if you don't have access to this fine machine never fear:

1. `mv <the teabag script> /usr/local/bin/teabag`
2. `sudo chmod 755 teabag`

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

For __help__ with any commands:

* `teabag help <command>`
