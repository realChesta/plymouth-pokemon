# Plymouth-Pokemon

This script generates a `two-step` theme for Plymouth that shows a randomly chosen Pokemon jumping until the boot process is finished.

## Usage
```shell
$ git clone https://github.com/realChesta/plymouth-pokemon.git
$ cd plymouth-pokemon
$ sudo sh pokemon-generator
```
*(`pokemon-generator` has to be run with elevated privileges.)*

Use **`pokemon-generator -a`** to automatically copy the generated theme into the themes directory and update the plymouth configuration. 

## Configuration

There are multiple variables that can easily be adjusted to tweak the functionality of the script:

* `PICK_RANGE` is the range of National PokeDex numbers to be included in the Pokemon selection.
* `ICON_LOCATION` determines where the the folder containing the icons is located.
* `ANIMATION_LENGTH` sets how many frames the animation should contain.
* `JUMP_HEIGHT` is the jump height in pixels (the canvas is 256x256)
* `DOUBLE_FINISH_ANIMATION` if this is set to `true`, the pokemon will jump twice before booting is completed (as opposed to once)