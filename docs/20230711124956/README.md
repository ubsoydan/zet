# Avoid POSIX regular expressions

POSIX regular expression classes might seem much more intuitive, self-explanatory, less troublesome due to range of options. But for an advanced web environment like today's, POSIX regex are highly insufficient. We have got emojis, kanjis, cyrillic chars etc. and POSIX is not able to cover all the new standards. For all those reasons, Unicode regex is way to go if possible (and if `grep` didn't do enough in that context).

unsolicited fun fact: Almost all regexes that you will encounter in languages on web world is based on PERL's regex convention. If you are using regex in JavaScript, Node.js or anything, you are most likely to be using PERL as well (in a way...). Look up PCRE for more info.
