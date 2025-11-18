# Get Zuericolors Palettes

Function to access color values of a specific zuericolors palette. To
see the available palettes, call
[`view_zuericolors()`](https://statistikstadtzuerich.github.io/zuericolors/reference/view_zuericolors.md).

## Usage

``` r
get_zuericolors(palette = names(palettes), nth)
```

## Arguments

- palette:

  Name of a specific palette; to see the available palettes, call
  [`view_zuericolors()`](https://statistikstadtzuerich.github.io/zuericolors/reference/view_zuericolors.md)

- nth:

  Position of a specific color in a palette, optional

## Value

the color(s) as hex strings

## Examples

``` r
# Get colors of palette 'qual12'
get_zuericolors("qual12")
#>  [1] "#3431DE" "#0A8DF6" "#23C3F1" "#7B4FB7" "#DB247D" "#FB737E" "#007C78"
#>  [8] "#1F9E31" "#99C32E" "#9A5B01" "#FF720C" "#FBB900"

# Get third color value of palette 'qual12'
get_zuericolors("qual12", 3)
#> [1] "#23C3F1"

# Get first three color values of palette 'qual12'
get_zuericolors("qual12", 1:3)
#> [1] "#3431DE" "#0A8DF6" "#23C3F1"
```
