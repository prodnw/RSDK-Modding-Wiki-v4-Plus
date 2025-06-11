# SetClassicFade

## Description
Adds a screen fade effect based on the `r`, `g`, `b` and `alpha` values, except it looks more like how it does in the classic games.

## Parameters
`r`

:   A value range of 0-255 for the color red.

`g`

:   A value range of 0-255 for the color green.

`b`

:   A value range of 0-255 for the color blue.

`alpha`

:   A value range of 0-255 for transparency, 255 being no transparency.

## Return Value
None.

## Syntax
```
SetClassicFade(int r, int g, int b, int alpha)
```

## Example
```
SetClassicFade(255, 255, 255, object.alpha)
```