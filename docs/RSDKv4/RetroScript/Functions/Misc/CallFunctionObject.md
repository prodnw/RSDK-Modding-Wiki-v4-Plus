# CallFunctionObject

!!! notice
    This is a new function added in RSDKv4+.

Calls the given function in a specified object, allowing you call from different objects.

## Parameters
`function`

:   The name (or numeric ID) of the object function to call.

`slot`

:   The index of the object to call from.

## Return Value
None.

## Syntax
```
CallFunctionObject(int function, int slot)
```

## Example
```
foreach (TypeName[Object], arrayPos0, ALL_ENTITIES)
    CallFunctionObject(MyObject_Function, arrayPos0)
next
```
