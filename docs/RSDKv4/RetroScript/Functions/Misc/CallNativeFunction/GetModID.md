# GetModID

!!! note
    This native function only exists in the RSDKv4 decompilation's mod loader. You can check if the function is usable by using the `USE_MOD_LOADER` platform flag.

!!! notice
    This is a new function added in RSDKv4+.

Gets the ID of the mod in the mod list (specifically where it's placed).

## Parameters
`ModName`

:   The exact name of the mod as it appears in the mod list.

## Return Value
Sets `checkResult` to the mod ID.

## Syntax
```
CallNativeFunction2(GetModID, 0, ModName)
```

## Example
```
CallNativeFunction2(GetModID, 0, "My Mod")
```

## Example (of checking is the mod you want to know is active)
```
CallNativeFunction2(GetModID, 0, "My Mod")
temp0 = checkResult
CallNativeFunction2(GetModActive, temp0, 0)
if checkResult == true
    [code goes here]
end if
```
