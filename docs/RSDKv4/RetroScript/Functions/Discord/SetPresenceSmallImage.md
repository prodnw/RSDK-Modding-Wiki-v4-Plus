# SetPresenceSmallImage

!!! notice
    This is a new function added in RSDKv4+.

Grabs an image from the art assets in your Discord application or a URL, and displays it on your status as a little icon on the bottom right of the main icon.

## Parameters
`imageName`

:   If you're using art from your Discord Application, then you'll want to input the exact same name as the art asset you're using. If you're using a URL, then it goes here.

`isUrl`

:   Determines if the image you want to use is from a URL or not.

## Return Value
None.

## Syntax
```
SetPresenceSmallImage(string imageName/url, bool isUrl)
```

## Example
```
SetPresenceSmallImage("sonic", false)
```
```
SetPresenceSmallImage("https://raw.githubusercontent.com/prodnw/mod-assets/refs/heads/main/Shadow%20-%20Discord%20Frontiers/sonic.png", true)
```