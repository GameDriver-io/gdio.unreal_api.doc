# ApiClient.DoubleClickObjectEx method

Use this function to interact with an object in game using a mouse double-click, combinated with key press operations. The total frame count execution of this operation is clickFrameCount + keysNumberOfFrames + modifiersNumberOfFrames

```csharp
public bool DoubleClickObjectEx(MouseButtons buttonId, string hierarchyPath, ulong clickFrameCount, 
    KeyCode[] keys = null, ulong keysNumberOfFrames = 5, int timeout = 30)
```

| parameter | description |
| --- | --- |
| buttonId | The mouse button to use for the double click operation. See MouseButtons. |
| hierarchyPath | The HierarchyPath for the GameObject to perform a double-click on. |
| clickFrameCount | The number of frames to double-click the specific object. |
| cameraHierarchyPath | Unused |
| keys | An array of [`KeyCode`](../KeyCode.md) keys to press during the click operation. |
| keysNumberOfFrames | The number of frames to press the keys parameter down. This parameter is not additive to the total count and is automatically accumulated by the function call. If this delay is longer than the frame count for all the key presses and click operation that the behavior of the result may not be what the user intends. |
| timeout | The number of seconds to wait for a response that the DoubleClickObjectEx request was processed. Input requests process asynchronously, so a response does NOT imply the input operation has completed. |

## Return Value

TRUE if the GameDriver agent successfully processed the request.

## Examples

```csharp
//Locates and clicks the first object with the name "Cube" for 30 frames with the left mouse button while holding the left-shift key for 3 frames, and the left-CTRL key for 5 frames.
            api.DoubleClickObjectEx(MouseButtons.LEFT,
                "//*[@name='Cube']", 30,
                new KeyCode[] { KeyCode.LeftControl }, 5,
                new KeyCode[] { KeyCode.LeftShift }, 3,
                500, 30);
```

## See Also

* enum [KeyCode](../KeyCode.md)
* class [ApiClient](../ApiClient.md)
* namespace [gdio.unreal_api](../../gdio.unreal_api.md)

<!-- DO NOT EDIT: generated by xmldocmd for gdio.unreal_api.dll -->
