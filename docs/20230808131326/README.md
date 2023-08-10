# 20230808131326
# Do not grep the cat

I've realized something. When I'm surfing thru StackOverflow for some answers,
everybody seems to know a solution but does not know the reason behind it.
Some answers consist pipe commands using both `grep` and `cat` as if `grep`
is not able to read files. `grep` is perfectly capable of reading files which
is what `cat` does essentially. Piping `grep` with `cat` is absolutely a bad
practice and unnecessary.

Instead of `cat file | grep "keyword"`, just use `grep "keyword" file`.
Do not grep the cat unless for some exceptional reason.
