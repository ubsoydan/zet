# the BLACKBOOK

* `sudo /sbin/dhclient` triggers dhcp client to assign another IP (multiple IPs possible), can be used if bridged network failed assigning one automatically.

* `command -v file` is same as `which`

* `set -o vi` vi keybindings option for shell

* `stty -a` teletype config listing - looks a bit like primal version of `screen` and `tmux`, also reminds me why `nano` is awful

* `vi` is basically visual mode of `ex`

* colon commands are a legacy of ed/ex

* `:!`, bang commands are just UNIX filters

* do not `grep` the `cat`

* pipelines are technically an implementation of functional programming

* in vim, `:linenumber!bangcommand` appends output at line

* `!}` formats paragraph

* exclamation mark in vim  runs external commands/scripts

* `:.,.+2!bash`

* quotes are painful in bash. use double quotes ama possible

* double quotes expand. for aliases, use single quotes

* functions and aliases violate `unix filters` requirements. filters are not
	executable within them, so they do not work.

* do not forget programs are binaries while scripts are interpreted

* functions are not only one kind. there are functions and procedures.
	functions are self contained, procedures are dependent on
	external factors.

* `find . -type d -maxdepth 3`

* `declare` is optional but considered as a good practice

* `\` backslash overrides aliases with original commands eg.`\date`  

* `echo $?` prompts exit status

* POSIX is dangerous, BASH is safe. Use double square brackets in bash.

* trivia. `[` is a binary (elf binary) --> ls `which [`

* using single square bracket `[`  is dangerous. good way to be pwned.
	heard it is vulnerable to shell injections via env variables.

* POSIX does not have `local` variable, BASH has.

* "AT&T Archives: The UNIX Operating System" https://youtu.be/tc4ROCJYbm0

* A good wrap of UNIX history "Is it time to rewrite the OS in Rust" https://youtu.be/HgtRAbE1nBM 

* Quite obscure `w` command displays who is logged in

* `set -o noclobber` for preventing unintended overwrites (>, >>)
	also can do `set -C`

* `-i` flag in context of `mv` to prevent overwrites

* `scp foo target:` i tend to forget colon, beware

* `ls -ld` looks up directory permission on current dir

* `stat -c '%a'` to see octal permissions

* trivia. `ls -l $(which sudo) to list permissions of sudo

* beware. `adduser` and `deluser` does not work on `redhat` distros.

* `find . -name '???'` finds files and dirs with any three letter name

* `find . -path '.git'` files/dirs with .git anywhere in the path

* `head -5 foo` and `tail -5 foo`

* `tac foo` reverse version of `cat`

* `wc -l` prints count of lines

* `nl` adds line numbers to stdout

* `tee /tmp/foo` writes to foo as well as to stdout

* Good playlist for the stuff that is not being taught formally  - https://www.youtube.com/@MissingSemester/videos

* O'reilly Mastering Regular Expressions

* trivia. geek code

* ed cheat sheet https://catonmat.net/ftp/ed.unix.text.editor.cheat.sheet.txt

* one of the best innovations of decade - SHELLCHECK shellcheck.net

* O'reilly UNIX Power Tools

* looks good as a BASH guide https://github.com/Idnan/bash-guide

* name may not seem bright but content is golden! https://itsfoss.com/learn-linux-for-free/

* use `command -v` in scripts instead of `which`

* never use extensions on executables on UNIX/Linux

* no floats in bash

* good old `$#`
