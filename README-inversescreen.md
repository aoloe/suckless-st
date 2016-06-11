# Inverse screen

## Use `setterm`

~~~.sh
setterm --inversescreen on
~~~

and in vim
~~~
:set background " dark | light "
~~~

## Patch the `st` colors

- invert the colors in `config.h`
- add `setenv("COLORFGBG", "15;0", 1);` in `st.c`

see:
- <http://unix.stackexchange.com/questions/245378/common-environment-variable-to-set-dark-or-light-terminal-background>
- <https://github.com/rocky/bash-term-background/blob/master/term-background.sh>
