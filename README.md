# abs-term-color

## SYNOPSIS

    $ abs get github.com/sysread/abs-term-color

    # example.abs
    color = require("abs-term-color")

    echo(color.green + color.on_cyan + "Enter your selection: " + color.reset)
    response = stdin()

## DESCRIPTION

`abs-term-color` builds and returns a hash of color escape strings suitable
for use on ANSI color terminals.

## LIMITATIONS

Requires the use of `echo -n -e` in order to build the escape sequences. This
is done in a single shell call.

## INSTALLATION

See the [official docs](https://www.abs-lang.org/misc/3pl)

## FUNCTIONS

### show()

Prints out each color's name, colorized in the colors, uh, _color_, one per
line.

## PROVIDES

Provides the following keyed escape codes:

#### ANSI: `[on_]ansi[0..255]`

    color.ansi4
    color.on_ansi7

#### Grey scale: `[on_]grey[0..23]`

    color.grey17
    color.on_grey3

#### RGB: `[on_]rgb[0..5][0..5][0..5]`

    color.rgb132
    color.on_rgb022

### 4-bit colors

#### `black`
#### `bright_black`
#### `on_black`
#### `on_bright_black`

#### `red`
#### `bright_red`
#### `on_red`
#### `on_bright_red`

#### `green`
#### `bright_green`
#### `on_green`
#### `on_bright_green`

#### `yellow`
#### `bright_yellow`
#### `on_yellow`
#### `on_bright_yellow`

#### `blue`
#### `bright_blue`
#### `on_blue`
#### `on_bright_blue`

#### `magenta`
#### `bright_magenta`
#### `on_magenta`
#### `on_bright_magenta`

#### `cyan`
#### `bright_cyan`
#### `on_cyan`
#### `on_bright_cyan`

#### `white`
#### `bright_white`
#### `on_white`
#### `on_bright_white`

## AUTHOR

Jeff Ober <sysread@fastmail.fm>

## COPYRIGHT AND LICENSE

This software is copyright (c) 2019 by Jeff Ober.
