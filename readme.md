# Approcah Script with speed control

A script to secure your approach from a target and avoid collision.

Showcase Video available here : [https://youtu.be/GqaKc3-UVYU](https://youtu.be/GqaKc3-UVYU)

## Guilded Server (better than Discord)

You can join me on Guilded for help or suggestions or requests by following that link : https://guilded.jericho1060.com

## Elements Required

- 1 Range Finder
- 1 Hybrid Button *(or any other type of button)*
- 1 Basic YOLOL Chip
- 1 YOLOL Chip Socket

## Button Fields

You must name your button `Approach`. If you are using a Hybrid Button, be sure to set the `ButtonOnStateValue` to `1` and the `ButtonOffStateValue` to `0`. The `ButtonStyle` must be set to `1` if you don't want to maintain the button.

![Button Fields](https://github.com/Jericho1060/sb-approach-speed-control/blob/main/pictures/Button_Fields.png?raw=true)

## Range Finder Fields

You are free to chose the 1st field of the Range Finder, it's only used to switch on or off. If you want th Range Finder to switch on at the same time you press the Approach button, name it `Approach` too. The second field is the max distance of the Range Finder, it must be named `rLength` and you are free to chose the value you want to set it. The last field must be named `rD`, it's the current length of the beam.

![Range Finder Fields](https://github.com/Jericho1060/sb-approach-speed-control/blob/main/pictures/RangeFinder_Fields.png?raw=true)

## Install the script

copy the content of the file `approach.yolol` on the basic chip

## options

On the 1st line of the script you can change 3 options:
```
a=15 b=150 c=1 if:rD>=:rLength thengoto1end goto:Approach+1
```

- `a` is the distance you want to stop from the target in meters
- `b` is the max speed your ship is capable. more this value is accurate, more the precision of the script will be good
- `c` is a brake factor. If you ship is missing a bit of braking power, you can increase that value, it will multiply the thrust send to your brake.

## Usage

Point the beam on a target (eg: an asteroid) and press the button. The ship will adjust its speed and brake to reach the specified distance from the target.

## Support or donation

if you like it, [<img src="https://github.com/Jericho1060/DU-Industry-HUD/blob/main/ressources/images/ko-fi.png?raw=true" width="150">](https://ko-fi.com/jericho1060)