# ApiClient class

```csharp
public class ApiClient
```

## Public Members

| name | description |
| --- | --- |
| [ApiClient](ApiClient/ApiClient.md)() | The default constructor. |
| event [LoggedMessage](ApiClient/LoggedMessage.md) |  |
| [CallMethod](ApiClient/CallMethod.md)(…) | Use this function to execute a Void method on an object. |
| [CallMethod&lt;T&gt;](ApiClient/CallMethod.md)(…) | Use this function to execute a method on an object. |
| [CaptureScreenshot](ApiClient/CaptureScreenshot.md)(…) | Use this function to capture a screenshot of the Game under test. |
| [Click](ApiClient/Click.md)(…) | Use this function to perform in-game mouse-clicks. (2 methods) |
| [ClickEx](ApiClient/ClickEx.md)(…) | Use this function to perform in-game mouse-clicks combined with key press operations. The total frame count of this operation is clickFrameCount + keysNumberOfFrames + modifiersNumberOfFrames (2 methods) |
| [ClickObject](ApiClient/ClickObject.md)(…) | Use this function to interact with an in-game object using mouse-clicks. |
| [ClickObjectEx](ApiClient/ClickObjectEx.md)(…) | Use this function to interact with an in-game object using mouse-clicks combined with key press operations. The total frame count execution of this operation is clickFrameCount + keysNumberOfFrames + modifiersNumberOfFrames. |
| [Connect](ApiClient/Connect.md)(…) | Use this function to connect to an Unreal game with GameDriver Agent configured and active. This function can connect to the unreal editor or a Standalone deployment of a game. |
| [DisableObjectCaching](ApiClient/DisableObjectCaching.md)(…) | Disable the use of object caching when doing HierarchyPath object resolution. |
| [Disconnect](ApiClient/Disconnect.md)() | Use this function to disconnect the API client from the Game. |
| [DoubleClick](ApiClient/DoubleClick.md)(…) | Use this function to perform in-game mouse double-clicks. (2 methods) |
| [DoubleClickEx](ApiClient/DoubleClickEx.md)(…) | Use this function to perform in game mouse double clicks combined with key press operations. The total frame count execution of this operation is clickFrameCount + keysNumberOfFrames + modifiersNumberOfFrames (2 methods) |
| [DoubleClickObject](ApiClient/DoubleClickObject.md)(…) | Use this function to interact with an object in game using a mouse double-click. |
| [DoubleClickObjectEx](ApiClient/DoubleClickObjectEx.md)(…) | Use this function to interact with an object in game using a mouse double-click, combinated with key press operations. The total frame count execution of this operation is clickFrameCount + keysNumberOfFrames + modifiersNumberOfFrames |
| [EnableObjectCaching](ApiClient/EnableObjectCaching.md)(…) | Enable the use of object caching when performing HierarchyPath object resolution. Object caching is per HierarchyPath stored in a IDictionary. If a matching HierarchyPath is already in the dictionary, then the stored object is returned. The only way to update a cached reference is for the reference to be garbage collected or flush the cache with [`FlushObjectLookupCache`](./ApiClient/FlushObjectLookupCache.md). |
| [FlushObjectLookupCache](ApiClient/FlushObjectLookupCache.md)(…) | If object caching is enabled, this method will request that the agent flush the cache being held for all object lookups. |
| [GetGameObject](ApiClient/GetGameObject.md)(…) | Get the UObject that evaluates from the provided HierarchyPath argument. |
| [GetLastFPS](ApiClient/GetLastFPS.md)() | This method returns the last frames per second that the API client has recieved from the GameDriver agent. |
| [GetObjectDistance](ApiClient/GetObjectDistance.md)(…) | This method returns the distance of two objects using vector subtraction. |
| [GetObjectFieldValue&lt;T&gt;](ApiClient/GetObjectFieldValue.md)(…) | This method returns the field or property value of an object. |
| [GetObjectList](ApiClient/GetObjectList.md)(…) | This method returns of a list of all GameObjects as returned by !:UnityEngine.GameObject.FindObjectsOfType(Type), where Type is UnityEngine.GameObject./&gt; (2 methods) |
| [GetObjectPosition](ApiClient/GetObjectPosition.md)(…) | Return the position of a specific object. |
| [GetSceneName](ApiClient/GetSceneName.md)(…) | Return the name of the current active scene. |
| [KeyPress](ApiClient/KeyPress.md)(…) | Use this function to send arbitrary button states to the game. Defaults to LEFT ALT/CTRL/SHIFT/WINDOWS(COMMAND) (2 methods) |
| [LoadLevel](ApiClient/LoadLevel.md)(…) | This method loads the scene, defined by the scene name passed as an argument. |
| [MouseDrag](ApiClient/MouseDrag.md)(…) | Perform a mouse drag operation. |
| [MouseMoveToObject](ApiClient/MouseMoveToObject.md)(…) | Move the mouse to the center of a specific object, identified by the HierarchyPath. |
| [MouseMoveToPoint](ApiClient/MouseMoveToPoint.md)(…) | Move the mouse to the destination vector. |
| [NavAgentMoveToPoint](ApiClient/NavAgentMoveToPoint.md)(…) | Move a NavAgent to a destination point. |
| [Raycast](ApiClient/Raycast.md)(…) | Perform a Raycast to a point to find out what is in that position. |
| [ReConnect](ApiClient/ReConnect.md)(…) | Use this function to disconnect and reconnect the API client to the Game. Useful after loading a new Scene when the agent is reloaded and requires reconnection. |
| [RegisterCollisionMonitor](ApiClient/RegisterCollisionMonitor.md)(…) | Register a collision monitor to recieve collision events on an object. |
| [RotateObject](ApiClient/RotateObject.md)(…) | Rotate an object defined by the HierarchyPath and rotated by a Quaternion. [https://scriptinghelpers.org/blog/how-to-think-about-quaternions](https://scriptinghelpers.org/blog/how-to-think-about-quaternions) for more information. (4 methods) |
| [SetInputFieldText](ApiClient/SetInputFieldText.md)(…) | Set the text of a TextBox or EditableText |
| [SetObjectFieldValue](ApiClient/SetObjectFieldValue.md)(…) | Set the field or property of an object. |
| [SetTimescale](ApiClient/SetTimescale.md)(…) | Use this function to set the play speed of the game. Can be used to speed up or slow down the game in order to improve test execution time. (https://docs.unity3d.com/ScriptReference/Time-timeScale.html) |
| [Tap](ApiClient/Tap.md)(…) | Tap the handheld device at the defined position. (2 methods) |
| [TapObject](ApiClient/TapObject.md)(…) | Tap an object. |
| [TouchInput](ApiClient/TouchInput.md)(…) | Send a raw TouchInput event to the game. (2 methods) |
| [UnregisterCollisionMonitor](ApiClient/UnregisterCollisionMonitor.md)(…) | Unregister the monitoring of collision events on a GameObject that has been previously registered for monitoring. |
| [Wait](ApiClient/Wait.md)(…) |  |
| [WaitForCollisionEvent](ApiClient/WaitForCollisionEvent.md)(…) | Wait for a collision event to fire on an element that is being monitored for collisions. If the method has been called before, there is the potential that another event was recieved before waiting on the event again. |
| [WaitForEmptyInput](ApiClient/WaitForEmptyInput.md)(…) | Wait for an Empty Input event to be received. |
| [WaitForObject](ApiClient/WaitForObject.md)(…) | Wait for an object to exist. |
| [WaitForObjectValue](ApiClient/WaitForObjectValue.md)(…) | Wait for an object to exist and have a specific value for a specified field/property. |

## See Also

* namespace [gdio.unreal_api](../gdio.unreal_api.md)

<!-- DO NOT EDIT: generated by xmldocmd for gdio.unreal_api.dll -->
