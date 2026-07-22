# SetMusicModifier

!!! notice
    This is a new function added in RSDKv4+.

Modifies the currently playing music track, allowing for different effects, with more to come soon.

## Parameters
`track`

:   The track ID to modify.

`modifier`

:   Which type of modifier to use.
:   `AUDIO_MOD_SPEED` edits the speed.

`data1`

:   The 1st effect of the modifier.
:   if `AUDIO_MOD_SPEED` then 100 is regular speed

`data2`

:   The 2nd effect of the modifier.

## Return Value
None.

## Syntax
```
SetMusicModifier(int track, int modifier, int data1, int data2)
```

## Example
```
SetMusicModifier(TRACK_STAGE, AUDIO_MOD_SPEED, 125, 0)
```
