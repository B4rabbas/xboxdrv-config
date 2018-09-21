# xboxdrv-config
A simple shell script for setting up xboxdrv evdev mappings for a given device, interactively
sudo evtest /dev/input/event6
ou si ca marche : sudo evtest /dev/input/event21


sudo xboxdrv --evdev /dev/input/event6 --evdev-absmap ABS_X=x1,ABS_Y=y1,ABS_Z=x2,ABS_RZ=y2,ABS_HAT0X=dpad_x,ABS_HAT0Y=dpad_y --axismap -Y1=Y1,-Y2=Y2 --evdev-keymap BTN_NORTH=x,BTN_SOUTH=y,BTN_C=a,BTN_EAST=b,BTN_TL2=back,BTN_TR2=start,BTN_WEST=lb,BTN_TL=rb,BTN_Z=lt,BTN_TR=rt,BTN_SELECT=tl,BTN_START=tr --mimic-xpad --silent &

Pour manette dualshock noname blanche :


BTN_C=a

BTN_EAST=b

BTN_TL2=back

BTN_TR2=start

BTN_WEST=lb

BTN_Z=rb

BTN_TL=lt

BTN_TR=rt

BTN_SELECT=tl

BTN_START=tr

ABS_X=x1

BTN_NORTH=x

BTN_SOUTH=y

ABS_Y=y1

ABS_Z=x2

ABS_RZ=y2

ABS_HAT0X=dpad_x

ABS_HAT0Y=dpad_y

-Y1=Y1

-Y2=Y2


sudo xboxdrv --evdev /dev/input/event6 --evdev-absmap ABS_X=x1,ABS_Y=y1,ABS_Z=x2,ABS_RZ=y2,ABS_HAT0X=dpad_x,ABS_HAT0Y=dpad_y --axismap -Y1=Y1,-Y2=Y2 --evdev-keymap BTN_NORTH=x,BTN_SOUTH=y,BTN_C=a,BTN_EAST=b,BTN_TL2=back,BTN_TR2=start,BTN_WEST=lb,BTN_Z=rb,BTN_TL=lt,BTN_TR=rt,BTN_SELECT=tl,BTN_START=tr --mimic-xpad --silent &
