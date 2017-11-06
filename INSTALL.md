This is a simple command line note taking app. Very useful if you want to quickly log what you are doing directly from your terminal.
The cool thing is: it accepts command/variable substitution, so you can actually capture and log output of commands and variables with your logs.

```
Usage: log [-h|-n|-s] [log entry]
-h      Print this help
-n      Do not escape characters when using multi-line.
-s      Save and push
```

### Examples

* To log using multiple lines, simple run `log` [ENTER]. All characters will be escaped, so bash variable substitution will not work. If you wish them to work, run `log -n` instead. Once you are done, press CTRL+D to save.
* To log inline, just type `log this is my inline log` [ENTER]. Variable substitutions will work here.

Every log entry gets automatically saved and pushed to your git repo.

### Installation instructions:

1. Fork it *as a private repo*.
2. Clone it.
3. Run `bin/install`
4. Follow the instructions on the screen about adding an alias to your `.bashrc` or `.bash_profile`