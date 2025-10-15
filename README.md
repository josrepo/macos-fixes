# macOS fixes
macOS has lots of annoying quirks and this repo contains some workarounds I have found to cope with them.

## Mouse button 4 and 5 
Using mouse `button 4` and `button 5` on a third-party mouse seems to fire the event twice, once on up and once on down.
Using [Karabiner-Elements](https://karabiner-elements.pqrs.org/) we can disable the down event so the button does not feel like it is double clicking.

Add the file `mouse-button-45-fix.json` to `~/.config/karabiner/assets/complex_modifications` to restore this behaviour.

## Swap @ and "
The "British English" version of the magic keyboard has the `@` and `"` keys in the American English locations.
If you are used to the British English layout, then by using [Karabiner-Elements](https://karabiner-elements.pqrs.org/) we can swap these so you can retain your muscle memory.

Add the file `swap-at-and-double-quote.json` to `~/.config/karabiner/assets/complex_modifications` to restore this behaviour.

## Alt + tab
`Command + tab` in macOS only switches between applications—not windows.
If you are used to the Windows style of `alt + tab`, there is a fantastic app called [AltTab](https://alt-tab-macos.netlify.app/) which enables this functionality.
It does not function entirely like Windows out of the box however, because releasing the `shift` key will select the previous window, whereas in Windows you would have to release `alt` as well.

Add the file `com.lwouis.alt-tab-macos.plist` to `~/Library/Preferences` to restore this behaviour.

## Replace eject with delete
The magic keyboard has a rarely used eject key above the backspace which I think is a much better place for the absent delete key.
Using [Karabiner-Elements](https://karabiner-elements.pqrs.org/) we can replace the eject key with a delete key which is much more useful.

Add the file `map-eject-to-delete.json` to `~/.config/karabiner/assets/complex_modifications` to restore this behaviour.

## Discrete scroll
The magic mouse benefits from scroll wheel acceleration, but if you prefer to use a third-party mouse, then it is undesirable.
Using [DiscreteScroll](https://github.com/emreyolcu/discrete-scroll) we can restore the normal behaviour of the mouse.

I have not provided a config file as the default settings are perfectly fine.
