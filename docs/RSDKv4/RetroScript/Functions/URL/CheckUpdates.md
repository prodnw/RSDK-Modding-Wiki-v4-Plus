# CheckUpdates

!!! notice
    This is a new function added in RSDKv4+, and requires cURL to use.

!!! note
    This isn't an automatic update checker, so whenever you update something that uses this function the GitHub page you're pulling from will automatically need to be updated

Checks for any differences between a number in the script and a number from the GitHub page you're pulling from.

How to set-up:

1. Make a new public GitHub repository.

2. Allow GitHub pages and auto-builds for your website containing the number to be built automatically.

3. Create a new `index.html` file, and in it type the number you want to use. For this example we'll go with `10`.

4. In the engine, go to where you want to check for updates and add this: CheckUpdates("`link`").

5. Where the word "link" is above, you put the link to your GitHub page.

6. The engine will get the value and store it in `checkResult`. If there was an error/you don't have internet it'll return as `-1`.

7. Add a checking for whether you need to update now, please look at the examples below for a better idea.

## Parameters
`link`

:   The link to your GitHub page, containing your version number.

## Return Value
Sets `checkResult` to the result.

## Syntax
```
CheckUpdates(char link)
```

## Example
```
private alias 5 : CURRENT_VERSION

switch object.state
case 0
    CheckUpdates("https://prodnw.github.io/DoF-version-number/")
    temp7 = checkResult

    object.state++
    break

case 1
    if CURRENT_VERSION != temp7
        object.versionCheck = true
    end if
    object.state++
    break

case 2
    if object.versionCheck == true
        // update notify menu
    else
        // continue as normal
    end if
end switch
```
