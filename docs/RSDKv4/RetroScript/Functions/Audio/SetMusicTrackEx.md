# SetMusicTrackEx

!!! notice
    This is a new function added in RSDKv4+.

Loads a music file in the given track slot with the given loop point.

## Parameters
`path`

:   The file path to load the music file from, relative to `Data/Music/`. The music file must be in OGG format.

`trackID`

:   The trackList slot to load the music in.

`loopPoint`

:   The track's loop point, in samples. `0` will disable looping, `1` will loop from the beginning of the track, and anything else is the sample to loop from.

`endLoopPoint`

:   The track's ending loop point, if the track reaches the specified point then it'll loop back to the starting loop point.

## Return Value
None.

## Syntax
```
SetMusicTrackEx(string path, int trackID, int loopPoint, int endLoopPoint)
```

## Example
```
SetMusicTrackEx("Test.ogg", 0, 1, 39380)
```
