# LoadVideo

!!! notice
    This is a new function added in RSDKv4+.

Loads and plays a video.

The compatible video formats and directory containing the videos vary depending on the version of the game/engine:

- `.ogv` files stored in `Data/Videos/`.
- `.rsv` files stored in `Data/Sprites/`.
- Sonic Origins: Videos are stored and handled by [Hedgehog Engine 2](/Games/SonicOrigins/HedgehogEngine2).

## Parameters
`Name`

:   The name of the video file to load. Unless you're loading an RSV file, the file extension should be excluded. See the list above for what path this is relative to.

`AudioTrack`

:   (WORKS ON OGV ONLY) Which audio track to play stored in the video file.

## Return Value
None.

## Syntax
```
LoadVideo(string Name, int AudioTrack)
```

## Examples
```
LoadVideo("Opening", 1)
```
```
LoadVideo("Cutscenes/Opening.rsv", 0)
```
