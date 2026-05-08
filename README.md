# Keykits

An example configuration that demonstrates how easy XKB configuration is when
you use arbitrary key configuration names (symbolic key codes) and assign them
to hardware keycode numbers.

Use the pre-supplied custom layout at `symbols/custom` and override
`keycodes/evdev`.

This is based on the German layout `de(nodeadkeys)`. You can change that in
`symbols/custom`.

With a recent libxkbcommon, just copy the `xkb` directory to `~/.config/xkb`,
select the custom layout, and you'll get:

- Cursor functions on level 3 on the right-hand of the home row.
- Level 3 shift on the Windows key.
- Control functionality on each side of the space bar.
- Alt functionality on the caps/return keys.
- Caps/Super (KDE "Meta) functionality on the left/right control keys.

Think of symbols/keycodes as virtual/hardware tending sides where you assemble
a set of personal configuration options in symbols, and where you instantiate
those on a keyboard in keycodes.

For further information, check out this great documentation:

[User-specific XKB configuration](https://who-t.blogspot.com/2020/09/user-specific-xkb-configuration-putting.html)

[libxkbcommon](https://xkbcommon.org/doc/current/index.html)
