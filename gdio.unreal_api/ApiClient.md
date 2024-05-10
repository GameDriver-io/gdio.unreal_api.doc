# ApiClient class

This class contains the api calls that allow you to interact with your game.

```csharp
public class ApiClient
```

## Public Members

| name | description |
| --- | --- |
| [ApiClient](ApiClient/ApiClient.md)() | The default constructor. |
| event [LoggedMessage](ApiClient/LoggedMessage.md) |  |
| event [ScriptSignal](ApiClient/ScriptSignal.md) |  |
| [CallMethod](ApiClient/CallMethod.md)(…) | Use this function to execute a Void method on an object. |
| [CallMethod&lt;T&gt;](ApiClient/CallMethod.md)(…) | Use this function to execute a method on an object. |
| [CaptureScreenshot](ApiClient/CaptureScreenshot.md)(…) | Use this function to capture a screenshot of the Game under test. |
| [Click](ApiClient/Click.md)(…) | Use this function to perform in-game mouse-clicks. (3 methods) |
| [ClickEx](ApiClient/ClickEx.md)(…) | Use this function to perform in-game mouse-clicks combined with key press operations. The total frame count of this operation is clickFrameCount + keysNumberOfFrames + modifiersNumberOfFrames (2 methods) |
| [ClickObject](ApiClient/ClickObject.md)(…) | Use this function to interact with an in-game object using mouse-clicks. |
| [ClickObjectEx](ApiClient/ClickObjectEx.md)(…) | Use this function to interact with an in-game object using mouse-clicks combined with key press operations. The total frame count execution of this operation is clickFrameCount + keysNumberOfFrames + modifiersNumberOfFrames. |
| [Connect](ApiClient/Connect.md)(…) | Use this function to connect to an Unreal game with GameDriver Agent configured and active. This function can connect to the unreal editor or a Standalone deployment of a game. |
| [CreateInputDevice](ApiClient/CreateInputDevice.md)(…) | Use this function to create a virtual input device (OculusHMD, etc). To be used with VRInput(), FloatInput(), Vector2Input() and other similar calls. |
| [DisableObjectCaching](ApiClient/DisableObjectCaching.md)(…) | Deprecated. Disable the use of object caching when doing HierarchyPath object resolution. |
| [Disconnect](ApiClient/Disconnect.md)() | Use this function to disconnect the API client from the Game. |
| [DoubleClick](ApiClient/DoubleClick.md)(…) | Use this function to perform in-game mouse double-clicks. (2 methods) |
| [DoubleClickEx](ApiClient/DoubleClickEx.md)(…) | Use this function to perform in game mouse double clicks combined with key press operations. The total frame count execution of this operation is clickFrameCount + keysNumberOfFrames + modifiersNumberOfFrames (2 methods) |
| [DoubleClickObject](ApiClient/DoubleClickObject.md)(…) | Use this function to interact with an object in game using a mouse double-click. |
| [DoubleClickObjectEx](ApiClient/DoubleClickObjectEx.md)(…) | Use this function to interact with an object in game using a mouse double-click, combinated with key press operations. The total frame count execution of this operation is clickFrameCount + keysNumberOfFrames + modifiersNumberOfFrames |
| [EnableObjectCaching](ApiClient/EnableObjectCaching.md)(…) | this method is deprecated and will be removed in a future api version |
| [FindLookAtRotation](ApiClient/FindLookAtRotation.md)(…) | Return a Rotator(Vector3) such that the new rotation points an object towards a target. |
| [FloatInputEvent](ApiClient/FloatInputEvent.md)(…) | Use this function to send arbitrary Float Input Event states to the game. |
| [FlushObjectLookupCache](ApiClient/FlushObjectLookupCache.md)(…) | Deprecated. If object caching is enabled, this method will request that the agent flush the cache being held for all object lookups. |
| [GetConnectedGameDetails](ApiClient/GetConnectedGameDetails.md)() | This method returns the details of the game that the API client is connected to. |
| [GetGameObject](ApiClient/GetGameObject.md)(…) | Get the LiteGameObject representing the UObject matching the provided HierarchyPath argument |
| [GetLastFPS](ApiClient/GetLastFPS.md)() | This method returns the last frames per second that the API client has recieved from the GameDriver agent. |
| [GetMethodList](ApiClient/GetMethodList.md)(…) | This method returns all the (reflected) Methods available for the passed in object. |
| [GetObjectDistance](ApiClient/GetObjectDistance.md)(…) | This method returns the distance of two objects using vector subtraction. |
| [GetObjectFieldValue](ApiClient/GetObjectFieldValue.md)(…) | This method returns the field or property value of an object. |
| [GetObjectFieldValue&lt;T&gt;](ApiClient/GetObjectFieldValue.md)(…) | This method returns the field or property value of an object. (2 methods) |
| [GetObjectList](ApiClient/GetObjectList.md)(…) | This method returns of a list of all Unreal UObject Objects in the World. (2 methods) |
| [GetObjectPosition](ApiClient/GetObjectPosition.md)(…) | Return the position of a specific object.The position returned is in worldspace coordinates for an actor or a component and screenspace coordinates for widgets. |
| [GetObjectRotation](ApiClient/GetObjectRotation.md)(…) | EGet the rotation of an in Game AActor or a USceneComponent as a Vector. |
| [GetPropertyList](ApiClient/GetPropertyList.md)(…) | This method returns a list of Properties for the passed in object. |
| [GetSceneName](ApiClient/GetSceneName.md)(…) | Return the name of the current active scene. |
| [GetWidgetRotation](ApiClient/GetWidgetRotation.md)(…) | Get the rotation of a UWidget as returned by GetRenderTransformAngle as a float value. |
| [KeyPress](ApiClient/KeyPress.md)(…) | Use this function to send arbitrary button states to the game. Defaults to LEFT ALT/CTRL/SHIFT/WINDOWS(COMMAND) (2 methods) |
| [LoadLevel](ApiClient/LoadLevel.md)(…) | This method loads the scene, defined by the scene name passed as an argument. |
| [MouseDrag](ApiClient/MouseDrag.md)(…) | Perform a mouse drag operation. |
| [MouseMoveToObject](ApiClient/MouseMoveToObject.md)(…) | Move the mouse to the center of a specific object, identified by the HierarchyPath. |
| [MouseMoveToPoint](ApiClient/MouseMoveToPoint.md)(…) | Move the mouse to the destination vector. |
| [NavAgentMoveToPoint](ApiClient/NavAgentMoveToPoint.md)(…) | Move a NavAgent to a destination point. |
| [Ping](ApiClient/Ping.md)(…) | Use this function to check for connectivity |
| [QuaternionInputEvent](ApiClient/QuaternionInputEvent.md)(…) | Use this function to send arbitrary Quaternion Event states to the game. |
| [Raycast](ApiClient/Raycast.md)(…) | Perform a Raycast to a point to find out what is in that position. |
| [ReConnect](ApiClient/ReConnect.md)(…) | Use this function to disconnect and reconnect the API client to the Game. Useful after loading a new Scene when the agent is reloaded and requires reconnection. |
| [RegisterCollisionMonitor](ApiClient/RegisterCollisionMonitor.md)(…) | Register a collision monitor to recieve collision events on an object. |
| [RemoveInputDevices](ApiClient/RemoveInputDevices.md)(…) | Use this function to remove all GameDriver virtual input devices |
| [RotateObject](ApiClient/RotateObject.md)(…) | Rotate an object defined by the HierarchyPath and rotated by a Quaternion. [https://scriptinghelpers.org/blog/how-to-think-about-quaternions](https://scriptinghelpers.org/blog/how-to-think-about-quaternions) for more information. (4 methods) |
| [Scroll](ApiClient/Scroll.md)(…) | Use this function to simulate mouse wheel scrolling. |
| [SetInputFieldText](ApiClient/SetInputFieldText.md)(…) | Set the text of a TextBox or EditableText |
| [SetObjectFieldValue](ApiClient/SetObjectFieldValue.md)(…) | Set the field or property of an object. |
| [SetObjectPosition](ApiClient/SetObjectPosition.md)(…) | Easily set the position of an AActor or USceneComponent in world coordinates. |
| [SetObjectRotation](ApiClient/SetObjectRotation.md)(…) | Easily rotate an AActor or a USceneComponent in world coordinates. |
| [SetTimescale](ApiClient/SetTimescale.md)(…) | Use this function to set the play speed of the game. Can be used to speed up or slow down the game in order to improve test execution time. (see https://docs.unrealengine.com/4.26/en-US/API/Runtime/Engine/Kismet/UGameplayStatics/SetGlobalTimeDilation/) |
| [SetWidgetRotation](ApiClient/SetWidgetRotation.md)(…) | Easily rotate a UWidget by passing in the angle. |
| [Tap](ApiClient/Tap.md)(…) | Tap the handheld device at the defined position. (2 methods) |
| [TapObject](ApiClient/TapObject.md)(…) | Tap an object. |
| [TouchInput](ApiClient/TouchInput.md)(…) | Send a raw TouchInput event to the game. (2 methods) |
| [UnregisterCollisionMonitor](ApiClient/UnregisterCollisionMonitor.md)(…) | Unregister the monitoring of collision events on a GameObject that has been previously registered for monitoring. |
| [UseWebSockets](ApiClient/UseWebSockets.md)(…) | Configure a WebSocket server for a client (GDIOAgent) to connect to. |
| [Vector2InputEvent](ApiClient/Vector2InputEvent.md)(…) | Use this function to send arbitrary Vector2 Event states to the game. |
| [Vector3InputEvent](ApiClient/Vector3InputEvent.md)(…) | Use this function to send arbitrary Vector3 Event states to the game. |
| [VRInput](ApiClient/VRInput.md)(…) | Convenience function to send arbitrary Vector3 with Quaternion Event states to the game for the HUD or controllers |
| [Wait](ApiClient/Wait.md)(…) | Sleep the api client for a certain number of milliseconds. See System.Threading.Thread.Sleep |
| [WaitForCollisionEvent](ApiClient/WaitForCollisionEvent.md)(…) | Wait for a collision event to fire on an element that is being monitored for collisions. If the method has been called before, there is the potential that another event was recieved before waiting on the event again. |
| [WaitForEmptyInput](ApiClient/WaitForEmptyInput.md)(…) | Wait for an Empty Input event to be received. |
| [WaitForObject](ApiClient/WaitForObject.md)(…) | Wait for an object to exist. |
| [WaitForObjectValue](ApiClient/WaitForObjectValue.md)(…) | Wait for an object to exist and have a specific value for a specified field/property. |

## See Also

* namespace [gdio.unreal_api](../gdio.unreal_api.md)

<!-- DO NOT EDIT: generated by xmldocmd for gdio.unreal_api.dll -->
