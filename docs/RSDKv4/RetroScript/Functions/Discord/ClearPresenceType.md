# ClearPresenceType

!!! notice
    This is a new function added in RSDKv4+.

Clears a specific part of your Discord presence.

## Parameters
`presenceType`

:   The different types of presence to be cleared.
:   0 for Details.
:   1 for Srare.
:   2 for Large Image.
:   3 for Large Text.
:   4 for Small Image.
:   5 for Small Text.

## Return Value
None.

## Syntax
```
ClearPresenceType(int presenceType)
```

## Example
```
ClearPresenceType(0)
```
