#!/bin/sh

# configure the displays
# @todo: detect quad monitors or default to one
xrandr --output DP-1 --mode 1920x1080 --pos 1080x0 --rotate inverted --output DVI-I-1 --mode 1920x1080 --pos 0x1080 --rotate left --output DVI-D-1 --mode 1920x1080 --pos 3000x1080 --rotate right --output HDMI-1 --mode 1920x1080 --pos 1080x1080 --rotate normal

# start the compositor
xcompmgr -cfF -D 3 &

# audio
pavucontrol &

# synapse
synapse -s &

# start awesome
exec awesome
