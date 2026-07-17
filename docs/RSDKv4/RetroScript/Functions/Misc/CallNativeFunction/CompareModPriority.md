# CompareModPriority

!!! note
    This native function only exists in the RSDKv4 decompilation's mod loader. You can check if the function is usable by using the `USE_MOD_LOADER` platform flag.

!!! notice
    This is a new function added in RSDKv4+.

Checks 2 specific mod and if one is higher or lower.

## Parameters
`Mod1`

:   The exact name of the mod as it appears in the mod list.

`Mod2`

:   The exact name of the other mod as it appears in the mod list.

## Return Value
If the `Mod2` mod listed has a higher priority, `checkResult` will be 1.
If the `Mod2` mod listed has a lower priority, `checkResult` will be 0.

## Syntax
```
CallNativeFunction2(CompareModPriority, Mod1, Mod2)
```

## Example
```
CallNativeFunction2(GetModID, 0, "My Mod 1")
temp0 = checkResult
CallNativeFunction2(GetModID, 0, "My Mod 2")
temp1 = checkResult
CallNativeFunction2(CompareModPriority, temp0, temp1)
```