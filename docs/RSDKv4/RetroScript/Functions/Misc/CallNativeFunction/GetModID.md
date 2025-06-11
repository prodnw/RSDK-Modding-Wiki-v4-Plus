# GetModID

!!! note
    This native function only exists in the RSDKv4 decompilation's mod loader. You can check if the function is usable by using the `USE_MOD_LOADER` platform flag.

## Description
Grabs the ID of any mod in your mod list and stores it in the checkResult

## Parameters
None.

## Return Value
Sets `checkResult` to the mod ID.

## Example
```
CallNativeFunction2(GetModID, 0, "(Mod Name)")
temp0 = checkResult
CallNativeFunction2(GetModActive, temp0, 0)
if checkResult == true
    (code here)
end if
```