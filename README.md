randcolor
======

**randcolor** outputs an RGB hex code with random hue and constant value. I
just use this so every new terminal's background color is random but dark,
so as to ensure that light text is always readable and easy to see.

## Usage

```
$ randcolor 0.1
#190018
```

How it's useful:

```
$ awk '/randcolor|urxvt/' /etc/i3/config    
set $urxvt exec urxvt -bg $(randcolor .05)
bindsym $mod+Return $urxvt
bindsym $mod+F1 $urxvt
```
