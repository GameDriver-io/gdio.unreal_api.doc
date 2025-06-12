# ApiClient class

The ApiClient class is the main entry point for interacting with GameDriver in both Unity and Unreal Engine applications. It implements all the API methods we need for connecting to the game and interacting with it.

```csharp
public class ApiClient
```

## Public Members

| name | description |
| --- | --- |
| [ApiClient](ApiClient/ApiClient.md)() | Constructor for the ApiClient. |
| event [LoggedMessage](ApiClient/LoggedMessage.md) |  |
| event [ScriptSignal](ApiClient/ScriptSignal.md) |  |
| event [UnityLoggedMessage](ApiClient/UnityLoggedMessage.md) |  |
| [CallMethod](ApiClient/CallMethod.md)(…) | Use this function to execute a Void method on an object. |
| [CallMethod&lt;T&gt;](ApiClient/CallMethod.md)(…) | Use this function to execute a method on an object. |
| [CaptureScreenshot](ApiClient/CaptureScreenshot.md)(…) | Use this function to capture a screenshot of the Game under test. |
| [Click](ApiClient/Click.md)(…) | Use this function to perform in-game mouse-clicks. (4 methods) |
| [ClickEx](ApiClient/ClickEx.md)(…) | Use this function to perform in-game mouse-clicks combined with key press operations. The total frame count of this operation is clickFrameCount + keysNumberOfFrames + modifiersNumberOfFrames (2 methods) |
| [ClickObject](ApiClient/ClickObject.md)(…) | Use this function to interact with an in-game object using mouse-clicks. |
| [ClickObjectEx](ApiClient/ClickObjectEx.md)(…) | Use this function to interact with an in-game object using mouse-clicks combined with key press operations. The total frame count execution of this operation is clickFrameCount + keysNumberOfFrames + modifiersNumberOfFrames. |
| [Connect](ApiClient/Connect.md)(…) | Use this void function to connect to an Unreal game with GameDriver Agent configured and active. The default port is 15505. |
| [ConsoleCommand](ApiClient/ConsoleCommand.md)(…) | Pass an unreal command to the Unreal Console. https://dev.epicgames.com/documentation/en-us/unreal-engine/unreal-engine-console-commands-reference |
| [CreateInputDevice](ApiClient/CreateInputDevice.md)(…) | Use this function to create a virtual input device (OculusHMD, etc). To be used with VRInput(), FloatInput(), Vector2Input() and other similar calls. |
| [CreateObjectRef](ApiClient/CreateObjectRef.md)(…) | Instantiate an Object (AActor or UObject) using its `Type` and Constructor params if any and store it's reference as an ObjectRef. (3 methods) |
| [DebugCommand](ApiClient/DebugCommand.md)(…) | Test the underlying debugger |
| [DictionariesToGameObjects](ApiClient/DictionariesToGameObjects.md)(…) |  |
| [DisableObjectCaching](ApiClient/DisableObjectCaching.md)(…) | Deprecated. Disable the use of object caching when doing HierarchyPath object resolution. |
| [Disconnect](ApiClient/Disconnect.md)() | Use this function to disconnect the API client from the Game. |
| [DoubleClick](ApiClient/DoubleClick.md)(…) | Use this function to perform in-game mouse double-clicks. (2 methods) |
| [DoubleClickEx](ApiClient/DoubleClickEx.md)(…) | Use this function to perform in game mouse double clicks combined with key press operations. The total frame count execution of this operation is clickFrameCount + keysNumberOfFrames + modifiersNumberOfFrames (2 methods) |
| [DoubleClickObject](ApiClient/DoubleClickObject.md)(…) | Use this function to interact with an object in game using a mouse double-click. |
| [DoubleClickObjectEx](ApiClient/DoubleClickObjectEx.md)(…) | Use this function to interact with an object in game using a mouse double-click, combinated with key press operations. The total frame count execution of this operation is clickFrameCount + keysNumberOfFrames + modifiersNumberOfFrames |
| [DrawDebugSphere](ApiClient/DrawDebugSphere.md)(…) | Use this function to draw a location in 3D space. Useful for debugging collisisons, and location based events. Based on static internal Unreal method, DrawDebugSphere is not intended for production use. |
| [EnableObjectCaching](ApiClient/EnableObjectCaching.md)(…) | this method is deprecated and will be removed in a future api version |
| [FindLookAtRotation](ApiClient/FindLookAtRotation.md)(…) | Return a Rotator(Vector3) such that the new rotation points an object towards a target. |
| [FloatInputEvent](ApiClient/FloatInputEvent.md)(…) | Send arbitrary Float Input Event states to the game. |
| [FlushObjectLookupCache](ApiClient/FlushObjectLookupCache.md)(…) | Deprecated. If object caching is enabled, this method will request that the agent flush the cache being held for all object lookups. |
| [GetConnectedGameDetails](ApiClient/GetConnectedGameDetails.md)() | This method returns the details of the game that the API client is connected to. |
| [GetGameObject](ApiClient/GetGameObject.md)(…) | Get the LiteGameObject representing the UObject matching the provided HierarchyPath argument |
| [GetLastFPS](ApiClient/GetLastFPS.md)() | This method returns the last frames per second that the API client has recieved from the GameDriver agent. |
| [GetMethodList](ApiClient/GetMethodList.md)(…) | Returns a dictionary of the methods attached to the target object. The key of the dictionary is a string representing the method signature. The value of the dictionary is the hierarchy path of the object the method is attached to. |
| [GetObjectDistance](ApiClient/GetObjectDistance.md)(…) | This method returns the distance of two objects using vector subtraction. |
| [GetObjectFieldValue](ApiClient/GetObjectFieldValue.md)(…) | This method returns the field or property value of an object. |
| [GetObjectFieldValue&lt;T&gt;](ApiClient/GetObjectFieldValue.md)(…) | This method returns the field or property value of an object. (2 methods) |
| [GetObjectList](ApiClient/GetObjectList.md)(…) | This method returns of a list of all Unreal UObject Objects in the World. (2 methods) |
| [GetObjectPosition](ApiClient/GetObjectPosition.md)(…) | Return the position of a specific object.The position returned is in worldspace coordinates for an actor or a component and screenspace coordinates for widgets. |
| [GetObjectRotation](ApiClient/GetObjectRotation.md)(…) | Get the rotation of an in Game AActor or a USceneComponent as a Vector. |
| [GetPropertyList](ApiClient/GetPropertyList.md)(…) | Returns a dictionary of the properties and fields attached to the target object. The key of the dictionary is the hierarchy path of the property. The value of the dictionary is the value of the property represented as a string. |
| [GetSceneName](ApiClient/GetSceneName.md)(…) | Return the name of the current active scene. |
| [GetWidgetRotation](ApiClient/GetWidgetRotation.md)(…) | Get the rotation of a UWidget as returned by GetRenderTransformAngle as a float value. |
| [KeyPress](ApiClient/KeyPress.md)(…) | Use this function to send arbitrary button states to the game. Defaults to LEFT ALT/CTRL/SHIFT/WINDOWS(COMMAND) (2 methods) |
| [LoadLevel](ApiClient/LoadLevel.md)(…) | This method loads the scene, defined by the scene name passed as an argument. |
| [MouseDrag](ApiClient/MouseDrag.md)(…) | Perform a mouse drag operation. |
| [MouseMoveToObject](ApiClient/MouseMoveToObject.md)(…) | Move the mouse to the center of a specific object, identified by the HierarchyPath. |
| [MouseMoveToPoint](ApiClient/MouseMoveToPoint.md)(…) | Move the mouse to the destination vector. |
| [NavAgentMoveToPoint](ApiClient/NavAgentMoveToPoint.md)(…) | Move a NavAgent to a destination point. |
| [Ping](ApiClient/Ping.md)(…) | Internal (void returning) function to maintain connectivity. Not called by users. |
| [QuaternionInputEvent](ApiClient/QuaternionInputEvent.md)(…) | Use this function to send arbitrary Quaternion Event states to the game. |
| [Raycast](ApiClient/Raycast.md)(…) | Perform a Raycast to a point to find out what is in that position. |
| [ReconfigurePort](ApiClient/ReconfigurePort.md)(…) | Reconfigure the agent to use a new port. |
| [ReConnect](ApiClient/ReConnect.md)(…) | Use this function to disconnect and reconnect the API client to the Game. Useful after loading a new Scene when the agent is reloaded and requires reconnection. |
| [RegisterCollisionMonitor](ApiClient/RegisterCollisionMonitor.md)(…) | Register a collision monitor to recieve collision events on an object. |
| [RemoveInputDevices](ApiClient/RemoveInputDevices.md)(…) | Use this function to remove all GameDriver virtual input devices |
| [RemoveObjectRef](ApiClient/RemoveObjectRef.md)(…) | Remove an objectRef |
| [RotateObject](ApiClient/RotateObject.md)(…) | Rotate an object defined by the HierarchyPath and rotated by a Quaternion. [https://scriptinghelpers.org/blog/how-to-think-about-quaternions](https://scriptinghelpers.org/blog/how-to-think-about-quaternions) for more information. (4 methods) |
| [Scroll](ApiClient/Scroll.md)(…) | Use this function to simulate mouse wheel scrolling. |
| [SetInputFieldText](ApiClient/SetInputFieldText.md)(…) | Set the text of a TextBox or EditableText |
| [SetObjectFieldValue](ApiClient/SetObjectFieldValue.md)(…) | Set the field or property of an object. |
| [SetObjectPosition](ApiClient/SetObjectPosition.md)(…) | Easily set the position of an AActor or USceneComponent in world coordinates. |
| [SetObjectRotation](ApiClient/SetObjectRotation.md)(…) | Easily rotate an AActor or a USceneComponent in world coordinates. |
| [SetTimescale](ApiClient/SetTimescale.md)(…) | Use this function to set the play speed of the game. Can be used to speed up or slow down the game in order to improve test execution time. (see https://docs.unrealengine.com/4.26/en-US/API/Runtime/Engine/Kismet/UGameplayStatics/SetGlobalTimeDilation/) |
| [SetWidgetRotation](ApiClient/SetWidgetRotation.md)(…) | Easily rotate a UWidget by passing in the angle. |
| [StartEditorPlay](ApiClient/StartEditorPlay.md)(…) |  |
| [StopEditorPlay](ApiClient/StopEditorPlay.md)(…) | Stop a game from playing in the Editor, if it is currently in Play mode. |
| [Tap](ApiClient/Tap.md)(…) | Tap the handheld device at the defined position. (2 methods) |
| [TapObject](ApiClient/TapObject.md)(…) | Tap an object. |
| [ToggleEditorPause](ApiClient/ToggleEditorPause.md)(…) |  |
| [ToggleEditorPlay](ApiClient/ToggleEditorPlay.md)(…) |  |
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
| static [AUTOPLAY_BROADCAST_ADDR](ApiClient/AUTOPLAY_BROADCAST_ADDR.md) | The broadcast address to use for sending out AutoPlay requests. The default is for localhost: 127.0.0.1 |
| static [AUTOPLAY_DEFAULT_PORT](ApiClient/AUTOPLAY_DEFAULT_PORT.md) | The default AUTOPLAY port to use when searching for running games. This port is configured in the Unity preferences. |
| static [AUTOPLAY_ENABLED](ApiClient/AUTOPLAY_ENABLED.md) | NOT IN USE. |
| static [AUTOPLAY_RECEIVE_PORT](ApiClient/AUTOPLAY_RECEIVE_PORT.md) | The port to listen for responses from the AutoPlay plugin running in Unity. Due to loopback limitations, this port must be different than the [`AUTOPLAY_DEFAULT_PORT`](./ApiClient/AUTOPLAY_DEFAULT_PORT.md) |

## Protected Members

| name | description |
| --- | --- |
| virtual [IsRecorder](ApiClient/IsRecorder.md) { get; } |  |
| [client](ApiClient/client.md) |  |
| event [MessageReceived](ApiClient/MessageReceived.md) | Passthrough event handler for for Api Extensions, eg: Recorder |
| [SendMessage](ApiClient/SendMessage.md)(…) | Internal Method used by api extensions to send messages to the GDIOAgent. |

## Examples

```csharp
//Instantiate the gamedriver api before using it
ApiClient api = new ApiClient();

```

## See Also

* namespace [gdio.unreal_api](../gdio.unreal_api.md)

<!-- DO NOT EDIT: generated by xmldocmd for gdio.unreal_api.dll -->
