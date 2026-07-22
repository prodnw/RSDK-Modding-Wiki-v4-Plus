# VibrateController

!!! notice
    This is a new function added in RSDKv4+.

Vibrates your controller.

## Parameters
`controllerID`

:   The controller to vibrate. `-1` to vibrate all, `0` for controller 1, `1` for controller 2, etc.

`intensity`

:   How strong the vibration is.

`timeMS`

:   How long the vibration will last, which are converted to milliseconds by the engine.

## Return Value
None.

## Syntax
```
VibrateController(int controllerID, int intensity, int timeMS)
```

## Example
```
VibrateController(0, 2500, 100)
```
