# fixscr
Screen Pattern setup for screens on Unix Systems

### Setup your screens

Based on patterns that you can write on ~/.fixscr you can define how your screen will
be setup with only one short command: `fixscr`.

When you use multiple monitors, you know that no operating system guess and setup your screen
correctly. Or sometimes you want only to use one screen on a defined setup.

That is when i build this small program, is a Python software that you can define some
patterns to your screen setup, just like a simplified `xorg.conf` and then you can easly change
between them

### How it works

You can just write a simple config file at `~/.fixscr` and all the patterns save there will
be available in fixscr.

The config file is really simple and reminds a simple `xorg.conf` file.

You can see the example `fixscr.example` inside this repository or see the wiki where
every option is available.

Then you just type `fixscr pattern` or `fixscr` in any terminal emulator or execute dialog (ALT+F2) to load a screen setup.

### What can i define

You can define, in only one pattern, the setup of any or all of your screens/monitor. The setup include resolution, refresh rate, brightness, if the screen is on or off and many more.

And you can define as many patterns as you want.

I have a default pattern where my laptop screen and my main monitor is on, and other that if the main monitor is plugged in it shuts down the laptop screen for playing games, called `games`. And i can simply call `fixscr games` to switch.

### How to use

4 Easy steps:

1. Make sure that you have all [dependencies](#dependencies) shown below.
2. Copy the fixscr file to your executable path (my recommendation is `/usr/local/bin`).
3. Create a `~/fixscr` with your patterns following the example and the wiki.
4. You're Ready.

### Dependencies

fixscr is written using Python and some core libraries. Currently it needs at least Python 2.7 installed (all modern unix system should have this available as a package, except gentoo haha ;).

fixscr also need some core python libraries:

* `subpcorcess`
* `sys`
* `os`
* `configparser`
* `time`

Besides Python, fixscr also needs `xrandr` utility from xorg. fixscr uses `xrandr` and probabily will not work with other window systems such as wayland.

### Licensing

fixscr is distributed under [GPLv3](https://www.gnu.org/licenses/gpl-3.0.en.html), you can find a copy of the license at LICENSE file.

In short, non-legal, terms this license has the freedoms:
* to use the software for any purpose,
* to change the software to suit your needs,
* to share the software with your friends and neighbors, and
* to share the changes you make.

##### Legal information

>Copyright (C) 2017  Artur 'h0m3' Paiva

>This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

>This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

>You should have received a copy of the GNU General Public License
along with this program.  If not, see <http://www.gnu.org/licenses/>.

>Feel free to contact me at dr.hoome@gmail.com.
