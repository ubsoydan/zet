# Portable script with env as a shebang

...and ultra insecure cases that it brings.

Using `#!/usr/bin/env python3` in shebang for a script might seem like a convenient practice, saves you the trouble of locating exact path of related interpreter. So it can work in any system, in any OS hassle-free.

-   `env` will look up to find ANY `python3` among the folders

But it raises some serious security concerns as well. Any user (or a hacker in this context) with privileges on the system can manipulate the path `...bin/python3` with malicious program so any script you try to run with it might compromise your system, your user, your privileges, everything. That's why it's not so wise to go with `env` approach.

If you really consider to use `env` for some reason, for it to be secure as much as hard path, you need to have users put their binary at pre-determined location or create a link symbolic/hard link or whatever. Otherwise, it's a security issue.
