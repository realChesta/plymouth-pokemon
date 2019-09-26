# Plymouth-Pokemon

This script generates a `two-step` theme for Plymouth that shows a randomly chosen Pokemon jumping until the boot process is finished.

Icons are from [oakdex-pokedex-sprites](https://github.com/jalyna/oakdex-pokedex-sprites/).

## Usage
```shell
$ git clone https://github.com/realChesta/plymouth-pokemon.git
$ cd plymouth-pokemon
$ sudo sh pokemon-generator
```
*(`pokemon-generator` has to be run with elevated privileges.)*

Use **`pokemon-generator -u`** to automatically copy the generated theme into the themes directory and **u**pdate the plymouth configuration. 

The option `-k` instructs the script to **k**eep the temporarily created resized pokemon image (`$TEMP_IMG`).

The option `-p` makes the script keep a `pokenum-prev.txt` file containing the number of the previousy generated Pokemon.

### Suggestion

Run `pokemon-generator -u` once per boot and enjoy a new Pokemon every time you boot!

## Configuration

There are multiple variables in the script that can easily be adjusted to tweak its functionality:

* `PICK_RANGE` is the range of National PokeDex numbers to be included in the Pokemon selection.
* `ICON_LOCATION` determines where the the folder containing the icons is located.
* `ANIMATION_LENGTH` sets how many frames the animation should contain.
* `JUMP_HEIGHT` is the jump height in pixels (the canvas is 256x256)
* `DOUBLE_FINISH_ANIMATION` if this is set to `true`, the pokemon will jump twice before booting is completed (as opposed to once)
