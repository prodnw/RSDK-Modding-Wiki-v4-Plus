# GetModAuthorURL

!!! note
    This native function only exists in the RSDKv4 decompilation's mod loader. You can check if the function is usable by using the `USE_MOD_LOADER` platform flag.

!!! notice
    This is a new function added in RSDKv4+.

Adds a text entry to `menu` with a mod's author URL as the text.

## Parameters
`menu`

:   The menu to add the text to. `MENU_1` or `MENU_2` are valid.

`highlightEntry`

:   Determines if the text will always be highlighted.

`id`

:   The ID of the mod to get the author URL of.

`unused`

:   Unused variable.

## Return Value
None.

## Syntax
```
CallNativeFunction4(GetModAuthorURL, int menu, int highlightEntry, int id, int unused)
```

## Example
```
CallNativeFunction4(GetModAuthorURL, MENU_1, false, 0, 0)
```
