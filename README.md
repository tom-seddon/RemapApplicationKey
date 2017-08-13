# Remap Application Key

This Automator app turns your PC keyboard's right-hand Application key
into a right-hand Command key.

It's intended for use in your login items list, so that it runs when
you log in. To try it out, just double click. The effect persists
until you reboot.

Requires Mac OS X Sierra.

# Why

I was moved to do this because my keyboard (MS Natural 4000) has a
Windows key between Left Control and Left Alt, and an Application key
in the corresponding right-hand spot. This makes sense for Windows,
where a right-hand Windows key would be mostly unnecessary, but it's
not so hot for OS X, which can benefit from two Command keys. (I mouse
left-handed, too, which doesn't help.)

I've been using Karabiner-Elements to do this remapping in Sierra, but
it has
[a bug whereby keys become stuck](https://github.com/tekezo/Karabiner-Elements/issues/545)
that I keep running into.

# How

It uses
[hidutil](https://developer.apple.com/library/content/technotes/tn2450/_index.html)
to remap key 0x65 to key 0xe7.
