# ZMK Keymap for Kangjun's keyboard 

- zmk keymap (based on Miryoku keymap)
- 3x5+3 split
- Qwerty layout
- 3x5+3 split keyboard
- working with mac OS yabai & skhd [Checkout my dotfiles]()

## Build

This repository doesn't include github action.

You need to clone zmk firmware and build it or use your own github action.

### Build locally
- [Setup build](https://zmk.dev/docs/development/setup)
- Clone this repository
- Clone [zmk firmware](https://github.com/zmkfirmware/zmk)
- `cd zmk/app`
- Build keymap
  - west build -d build/right -b <board_name> -- -DSHIELD=<shield_name>_right -DZMK_CONFIG="/path/to/this-repo/config"
  - west build -d build/left -b <board_name> -- -DSHIELD=<shield_name>_left -DZMK_CONFIG="/path/to/this-repo/config"
- Upload firmware
  - connect keyboard to your computer
  - double press reset button on your keyboard
  - drag and drop `build/<left|right>/zephyr/zmk.uf2` to your keyboard
  - do same thing for another side
  



## Layout

- Base Layer
- Mouse
- Nav
- Media 
- Sym
- Num
- [WM](#WM)
- Fun

'Image here'



## WM

### Base Keys
| Name         | Description                | Binding      |
| ------------ | -------------------------- | ------------ |
| D1           | Focus to desktop 1         | F13          |
| D2           | Focus to desktop 2         | F14          |
| D3           | Focus to desktop 3         | F15          |
| D4           | Focus to desktop 4         | F16          |
| D5           | Focus to desktop 5         | F17          |
| D6           | Focus to desktop 6         | F18          |
| D7           | Focus to desktop 7         | F19          |
|              |                            |              |
| W ⬅          | Focus to window left       | alt+F13      |
| W ⬆          | Focus to window up         | alt+F14      |
| W ⬇          | Focus to window down       | alt+F15      |
| W ⮕          | Focus to window right      | alt+F16      |
|              |                            |              |
| Dis ⬅        | Focus to display left      | alt+F17      |
| Dis ⬆        | Focus to display up        | alt+F18      |
| Dis ⬇        | Focus to display down      | alt+F19      |
| Dis ⮕        | Focus to display right     | ctrl+F13     |
|              |                            |              |
| W Size ⬅     | Increase window size left  | ctrl+F14     |
| W Size ⬆     | Increase window size up    | ctrl+F15     |
| W Size ⬇     | Increase window size down  | ctrl+F16     |
| W Size ⮕     | Increase window size right | ctrl+F17     |
|              |                            |              |
| D ⬅          | Focus to previous desktop  | ctrl+F18     |
| D ⬆          | Focus to next desktop      | ctrl+F19     |
|              |                            |
| X Mirror     | Mirror window horizontally | ctrl+alt+F13 |
| Y Mirror     | Mirror window vertically   | ctrl+alt+F14 |
| W Rotate CW  | Rotate window clockwise    | ctrl+alt+F15 |
| W Float/Grid | Toggle window float/grid   | ctrl+alt+F16 |
| W Max        | Toggle window maximum      | ctrl+alt+F17 |
| W Balance    | Toggle window maximum      | ctrl+alt+F18 |



### Combo Actions
| Name              | Description                     | Binding           |
| ----------------- | ------------------------------- | ----------------- |
| (shift+) D1       | Move window to desktop 1        | (shift+) F20      |
| (shift+) D2       | Move window to desktop 2        | (shift+) F13      |
| (shift+) D3       | Move window to desktop 3        | (shift+) F14      |
| (shift+) D4       | Move window to desktop 4        | (shift+) F15      |
| (shift+) D5       | Move window to desktop 5        | (shift+) F16      |
| (shift+) D6       | Move window to desktop 6        | (shift+) F17      |
| (shift+) D7       | Move window to desktop 7        | (shift+) F18      |
|                   |                                 |                   |
| (shift+) W ⬅      | Move window to left             | (shift+) alt+F13  |
| (shift+) W ⬆      | Move window to up               | (shift+) alt+F14  |
| (shift+) W ⬇      | Move window to down             | (shift+) alt+F15  |
| (shift+) W ⮕      | Move window to right            | (shift+) alt+F16  |
|                   |                                 |                   |
| (shift+) Dis ⬅    | Move window to display left     | (shift+) alt+F17  |
| (shift+) Dis ⬆    | Move window to display up       | (shift+) alt+F18  |
| (shift+) Dis ⬇    | Move window to display down     | (shift+) alt+F19  |
| (shift+) Dis ⮕    | Move window to display right    | (shift+) ctrl+F13 |
|                   |                                 |                   |
| (shift+) W Size ⬅ | Decrease window size left       | (shift+) ctrl+F14 |
| (shift+) W Size ⬆ | Decrease window size up         | (shift+) ctrl+F15 |
| (shift+) W Size ⬇ | Decrease window size down       | (shift+) ctrl+F16 |
| (shift+) W Size ⮕ | Decrease window size right      | (shift+) ctrl+F17 |
|                   |                                 |                   |
| (shift+) D ⬅      | Move window to previous desktop | (shift+) ctrl+F18 |
| (shift+) D ⬆      | Move window to next desktop     | (shift+) ctrl+F19 |




## See also
- [ZMK](https://zmk.dev/)
- [Miryoku zmk](https://github.com/manna-harbour/miryoku_zmk)
- [Corne keyboard (36-42 keys)](https://github.com/foostan/crkbd)
- [Totem keyboard (38 keys)](https://github.com/GEIGEIGEIST/TOTEM)
    - My first split keyboard
- [My dotfiles](https://github.com/gangjun06/dotfiles)

