# SetControllerLEDColour

!!! notice
    This is a new function added in RSDKv4+.

Changes the colour of the LED on PlayStation controllers.

## Parameters
`controllerID`

:   The controller to change the LED colour on. `0` for controller 1, `1` for controller 2, etc.

`r`

:   Red colour.

`g`

:   Green colour.

`b`

:   Blue colour.

## Return Value
None.

## Syntax
```
SetControllerLEDColour(int controllerID, int r, int g, ing b)
```

## Example
```
SetControllerLEDColour(0, 128, 128, 128)
```
