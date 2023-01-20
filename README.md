# BSD Berkley Software Distribution

# shell prompt
PROMPT='%n%f@%m%f %d%f %# '

# adapt screen
/bin/sh -c "xrandr --output $(xrandr | awk '/ connected/{print $1; exit; }') --auto"
