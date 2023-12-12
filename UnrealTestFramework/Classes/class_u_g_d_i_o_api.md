---
title: UGDIOApi

---

# UGDIOApi





Inherits from UObject

## Public Functions

|                | Name           |
| -------------- | -------------- |
| template <typenameT \> <br>bool | **[GetObjectFieldValue](class_u_g_d_i_o_api.md#function-getobjectfieldvalue)**(FString hierarchyPath, FString fieldName, T & value)<br>This method returns the field or property value of an object. (int, double, string & bool supported)  |
| template <typenameT \> <br>[bool](class_u_g_d_i_o_api.md#function-getobjectfieldvalue) | **[SetObjectFieldValue](class_u_g_d_i_o_api.md#function-setobjectfieldvalue)**([FString](class_u_g_d_i_o_api.md#function-getobjectfieldvalue) hierarchyPath, [FString](class_u_g_d_i_o_api.md#function-getobjectfieldvalue) fieldName, [T](class_u_g_d_i_o_api.md#function-getobjectfieldvalue) value)<br>Set the field or property of an object. (int, double, string & bool supported)  |
| [](class_u_g_d_i_o_api.md#function-getobjectfieldvalue) UObject * | **[GetGameObject](class_u_g_d_i_o_api.md#function-getgameobject)**([FString](class_u_g_d_i_o_api.md#function-getobjectfieldvalue) hierarchyPath)<br>Get the Object Reference matching the provided HierarchyPath argument, or NULL.  |
| [](class_u_g_d_i_o_api.md#function-getobjectfieldvalue)[TArray](class_u_g_d_i_o_api.md#function-getobjectfieldvalue)< UObject * > | **[GetObjectList](class_u_g_d_i_o_api.md#function-getobjectlist)**([FString](class_u_g_d_i_o_api.md#function-getobjectfieldvalue) hierarchyPath)<br>This method returns a TArray of all Unreal UObject matching the passed in HPath.  |
| [](class_u_g_d_i_o_api.md#function-getobjectfieldvalue)[bool](class_u_g_d_i_o_api.md#function-getobjectfieldvalue) | **[KeyPress](class_u_g_d_i_o_api.md#function-keypress)**([TArray](class_u_g_d_i_o_api.md#function-getobjectfieldvalue)< [FKey](class_u_g_d_i_o_api.md#function-getobjectfieldvalue) > keys, [int](class_u_g_d_i_o_api.md#function-getobjectfieldvalue) numberOfFrames)<br>Use this function to send arbitrary button states to the game.  |
| [](class_u_g_d_i_o_api.md#function-getobjectfieldvalue)[FString](class_u_g_d_i_o_api.md#function-getobjectfieldvalue) | **[getHierarchyPath](class_u_g_d_i_o_api.md#function-gethierarchypath)**(UObject * obj, [FString](class_u_g_d_i_o_api.md#function-getobjectfieldvalue) type)<br>Use this function to get the HierarchyPath of any vaid UObject.  |
| [](class_u_g_d_i_o_api.md#function-getobjectfieldvalue)[bool](class_u_g_d_i_o_api.md#function-getobjectfieldvalue) | **[Click](class_u_g_d_i_o_api.md#function-click)**([FKey](class_u_g_d_i_o_api.md#function-getobjectfieldvalue) MouseButton, [FVector2D](class_u_g_d_i_o_api.md#function-getobjectfieldvalue) location, [int](class_u_g_d_i_o_api.md#function-getobjectfieldvalue) numberOfFrames)<br>Use this function to perform in-game mouse-clicks.  |
| [](class_u_g_d_i_o_api.md#function-getobjectfieldvalue)[bool](class_u_g_d_i_o_api.md#function-getobjectfieldvalue) | **[ClickObject](class_u_g_d_i_o_api.md#function-clickobject)**([FKey](class_u_g_d_i_o_api.md#function-getobjectfieldvalue) MouseButton, [FString](class_u_g_d_i_o_api.md#function-getobjectfieldvalue) HPath, [int](class_u_g_d_i_o_api.md#function-getobjectfieldvalue) numberOfFrames)<br>Use this function to interact with an in-game object using mouse-clicks.  |
| [](class_u_g_d_i_o_api.md#function-getobjectfieldvalue)[bool](class_u_g_d_i_o_api.md#function-getobjectfieldvalue) | **[ClickObject](class_u_g_d_i_o_api.md#function-clickobject)**([FKey](class_u_g_d_i_o_api.md#function-getobjectfieldvalue) MouseButton, UObject * object, [int](class_u_g_d_i_o_api.md#function-getobjectfieldvalue) numberOfFrames)<br>Use this function to interact with an in-game object using mouse-clicks.  |
| [](class_u_g_d_i_o_api.md#function-getobjectfieldvalue)[bool](class_u_g_d_i_o_api.md#function-getobjectfieldvalue) | **[MouseMovetoPoint](class_u_g_d_i_o_api.md#function-mousemovetopoint)**([FVector2D](class_u_g_d_i_o_api.md#function-getobjectfieldvalue) destination, [int](class_u_g_d_i_o_api.md#function-getobjectfieldvalue) frameCount, [FVector2D](class_u_g_d_i_o_api.md#function-getobjectfieldvalue) origin)<br>Move the mouse to the destination vector.  |
| [](class_u_g_d_i_o_api.md#function-getobjectfieldvalue)[bool](class_u_g_d_i_o_api.md#function-getobjectfieldvalue) | **[MouseMovetoObject](class_u_g_d_i_o_api.md#function-mousemovetoobject)**([FString](class_u_g_d_i_o_api.md#function-getobjectfieldvalue) HPath, [int](class_u_g_d_i_o_api.md#function-getobjectfieldvalue) frameCount)<br>Move the mouse to the center of a specific object, identified by the HPath.  |
| [](class_u_g_d_i_o_api.md#function-getobjectfieldvalue)[bool](class_u_g_d_i_o_api.md#function-getobjectfieldvalue) | **[MouseMovetoObject](class_u_g_d_i_o_api.md#function-mousemovetoobject)**(UObject * obj, [int](class_u_g_d_i_o_api.md#function-getobjectfieldvalue) frameCount)<br>Move the mouse to the center of a specific object.  |
| [](class_u_g_d_i_o_api.md#function-getobjectfieldvalue)[bool](class_u_g_d_i_o_api.md#function-getobjectfieldvalue) | **[MouseDrag](class_u_g_d_i_o_api.md#function-mousedrag)**([FKey](class_u_g_d_i_o_api.md#function-getobjectfieldvalue) MouseButton, [FVector2D](class_u_g_d_i_o_api.md#function-getobjectfieldvalue) destination, [int](class_u_g_d_i_o_api.md#function-getobjectfieldvalue) frameCount, [FVector2D](class_u_g_d_i_o_api.md#function-getobjectfieldvalue) origin)<br>Perform a mouse drag operation.  |
| [](class_u_g_d_i_o_api.md#function-getobjectfieldvalue)[FVector](class_u_g_d_i_o_api.md#function-getobjectfieldvalue) | **[GetObjectPosition](class_u_g_d_i_o_api.md#function-getobjectposition)**([FString](class_u_g_d_i_o_api.md#function-getobjectfieldvalue) HPath, [CoordinateConversion](class_u_g_d_i_o_api.md#function-getobjectfieldvalue) coordinateSpace, [bool](class_u_g_d_i_o_api.md#function-getobjectfieldvalue) & valid)<br>Return the position of a specific object.The position returned is in worldspace coordinates for an actor or a component and screenspace coordinates for widgets.  |
| [](class_u_g_d_i_o_api.md#function-getobjectfieldvalue)[FVector](class_u_g_d_i_o_api.md#function-getobjectfieldvalue) | **[GetObjectPosition](class_u_g_d_i_o_api.md#function-getobjectposition)**(UObject * obj, [CoordinateConversion](class_u_g_d_i_o_api.md#function-getobjectfieldvalue) coordinateSpace, [bool](class_u_g_d_i_o_api.md#function-getobjectfieldvalue) & valid)<br>Return the position of a specific object.The position returned is in worldspace coordinates for an actor or a component and screenspace coordinates for widgets.  |
| [](class_u_g_d_i_o_api.md#function-getobjectfieldvalue)[bool](class_u_g_d_i_o_api.md#function-getobjectfieldvalue) | **[FloatInputEvent](class_u_g_d_i_o_api.md#function-floatinputevent)**([FKey](class_u_g_d_i_o_api.md#function-getobjectfieldvalue) key, [double](class_u_g_d_i_o_api.md#function-getobjectfieldvalue) value)<br>Use this function to simulate a KeyAxis float input (axis). Pass 0 to stop sending the event.  |

## Public Functions Documentation

### function GetObjectFieldValue

```cpp
template <typenameT >
static bool GetObjectFieldValue(
    FString hierarchyPath,
    FString fieldName,
    T & value
)
```

This method returns the field or property value of an object. (int, double, string & bool supported) 

**Parameters**: 

  * **hierarchyPath** The HierarchyPath of the object and field/property to be inspected.
  * **fieldName** The field/property name to retreieve the value for
  * **value** Out parameter that will contain an object of type T


**Template Parameters**: 

  * **T** The System.Type of the field or property to be inspected.


**Return**: True on success, false on error.



// Searches for an object named 'Player1' and gets the value of a integer field named _coins_

```cpp
int numCoins = UGDIOApi::GetObjectFieldValue<int>("/Player1", "coins");
```


### function SetObjectFieldValue

```cpp
template <typenameT >
static bool SetObjectFieldValue(
    FString hierarchyPath,
    FString fieldName,
    T value
)
```

Set the field or property of an object. (int, double, string & bool supported) 

**Parameters**: 

  * **hierarchyPath** The HierarchyPath to the object to set the field/property value.
  * **fieldName** The field or property name to set the value of.
  * **value** The value to set for the field/property.


**Return**: TRUE if the field/property was successfully set to the value.





```cpp
 // Change the newInt field to be 7.
UGDIOApi::SetObjectFieldValue<int>("//*[@tag='Player1']", "newInt", 7);
```


### function GetGameObject

```cpp
static  UObject * GetGameObject(
    FString hierarchyPath
)
```

Get the Object Reference matching the provided HierarchyPath argument, or NULL. 

**Parameters**: 

  * **hierarchyPath** The timeout in seconds to wait for a response that the request was processed by the GameDriver agent.
  * **timeout** The timeout in seconds to wait for a response that the request was processed by the GameDriver agent.


**Return**: The matching UObject, if it exists.





```cpp
UGDIOApi::GetGameObject("//*[@name='MyObject']")
```


### function GetObjectList

```cpp
static TArray< UObject * > GetObjectList(
    FString hierarchyPath
)
```

This method returns a TArray of all Unreal UObject matching the passed in HPath. 

**Parameters**: 

  * **hierarchyPath** The Hpath to use for the query


**Return**: a TArray of UObject* matching the query.



//Make sure only 1 object matches an HPath 

```cpp
TArray<UObject*> objects = UGDIOApi::GetObjectList("//mainCharacter");
if (objects.Num() == 1) { return true; }
return false;
```


### function KeyPress

```cpp
static bool KeyPress(
    TArray< FKey > keys,
    int numberOfFrames
)
```

Use this function to send arbitrary button states to the game. 

**Parameters**: 

  * **key** FKey indicating which key
  * **numberOfFrames** The number of frames to press and hold the keys for.


**Return**: TRUE if the GameDriver agent successfully processed the request.





```cpp
//Send events for the common W,A keys, maybe as input to a player controller. 
UGDIOApi::KeyPress(new KeyCode[] { KeyCode.W }, 15);
UGDIOApi::KeyPress(new KeyCode[] { KeyCode.A }, 15);
```


### function getHierarchyPath

```cpp
static FString getHierarchyPath(
    UObject * obj,
    FString type
)
```

Use this function to get the HierarchyPath of any vaid UObject. 

**Parameters**: 

  * **obj** The Object you want the HPath of
  * **type** "Absolute" or "Relative"


**Return**: The HierarchyPath of the Object as an FString





```cpp
//UObject* object is defined and assigned somewhere....
FString hpath = UGDIOApi::getHierarchyPath(object,"Absolute");
```


### function Click

```cpp
static bool Click(
    FKey MouseButton,
    FVector2D location,
    int numberOfFrames
)
```

Use this function to perform in-game mouse-clicks. 

**Parameters**: 

  * **MouseButton** The mouse button to use for the click operation.
  * **location** The [Vector2](class_u_g_d_i_o_api.md#function-getobjectfieldvalue) position to perform the mouse click.
  * **numberOfFrames** The number of frames to click the specific position.


**Return**: TRUE if the click was able to be simulated





```cpp
UGDIOApi::Click(MouseButtons.LEFT, new FVector2D (0, 0), 30); //Clicks the left mouse button at 0,0 for 30 frames
```


### function ClickObject

```cpp
static bool ClickObject(
    FKey MouseButton,
    FString HPath,
    int numberOfFrames
)
```

Use this function to interact with an in-game object using mouse-clicks. 

**Parameters**: 

  * **buttonId** The fKey for the mouse button to use for the click operation.
  * **HPath** The HierarchyPath for the GameObject to perform a click on.
  * **frameCount** The number of frames to click the specific object.


**Return**: TRUE if the HPath resolved and the click was able to be simulated





```cpp
UGDIOApi::ClickObject(MouseButtons.LEFT, "//*[@name='Cube']", 30);
```


### function ClickObject

```cpp
static bool ClickObject(
    FKey MouseButton,
    UObject * object,
    int numberOfFrames
)
```

Use this function to interact with an in-game object using mouse-clicks. 

**Parameters**: 

  * **MouseButton** The fKey for the mouse button to use for the click operation.
  * **object** A refernece to the object to perform a click on 
  * **frameCount** The number of frames to click the specific object.


**Return**: TRUE if the click was able to be simulated





```cpp
//UObject* object is defined and assigned somewhere....
UGDIOApi::ClickObject(MouseButtons.LEFT, object, 30);
```


### function MouseMovetoPoint

```cpp
static bool MouseMovetoPoint(
    FVector2D destination,
    int frameCount,
    FVector2D origin
)
```

Move the mouse to the destination vector. 

**Parameters**: 

  * **destination** Destination vector to move the mouse to.
  * **frameCount** The number of frames to complete the operaiton over.
  * **origin** The origin to start the mouse move operation. If null, the mouse move operation will begin at the current position of Input.mousePosition.


**Return**: TRUE if the method call was successfully processed by the GameDriver agent.





```cpp
//First get the position of an object named "Cube" on screen
FVector2D dest(1080, 100);
FVector2D origin(1080, 100);
UGDIOApi::MouseMovetoPoint(dest, 1000, origin);
```


### function MouseMovetoObject

```cpp
static bool MouseMovetoObject(
    FString HPath,
    int frameCount
)
```

Move the mouse to the center of a specific object, identified by the HPath. 

**Parameters**: 

  * **HPath** The HierarchyPath to move the mouse pointer to.
  * **frameCount** The number of frames to compelte the mouse move over.


**Return**: TRUE if the HPath is valid





```cpp
//Moves the mouse to the center of the object named "Cylinder" over 300 frames
UGDIOApi::MouseMovetoObject("//Cylinder", 300);
/code></example> 
```


### function MouseMovetoObject

```cpp
static bool MouseMovetoObject(
    UObject * obj,
    int frameCount
)
```

Move the mouse to the center of a specific object. 

**Parameters**: 

  * **obj** The obj to move the mouse pointer to.
  * **frameCount** The number of frames to complete the mouse move over.


**Return**: TRUE if the method call was successfully processed by the GameDriver agent.





```cpp
//Moves the mouse to the center of the object named "Cylinder" over 300 frames
//UObject* object is defined and assigned somewhere....
UGDIOApi::MouseMovetoObject(object, 300);
/code></example> 
```


### function MouseDrag

```cpp
static bool MouseDrag(
    FKey MouseButton,
    FVector2D destination,
    int frameCount,
    FVector2D origin
)
```

Perform a mouse drag operation. 

**Parameters**: 

  * **button** The mouse button as an FKey
  * **destination** The destination vector to drag the mouse to.
  * **frameCount** The number of frames taken to complete the drag operation.
  * **origin** The origin to start the drag operation. If null, the mouse drag operation will begin at the current position of Input.mousePosition.
  * **waitForEmptyInput** Wait for the empty input event to be returned from the agent before returning from the method call.


**Return**: TRUE if the requests was successfully processed by the GameDriver agent.





```cpp
//Drags the left mouse button to the position 180, 0 on the screen over 100 frames
FVector2D origin(100, 100);
FVector2D dest(180, 500);
UGDIOApi::MouseDrag(EKeys::LeftMouseButton, dest, 100, origin);
```


### function GetObjectPosition

```cpp
static FVector GetObjectPosition(
    FString HPath,
    CoordinateConversion coordinateSpace,
    bool & valid
)
```

Return the position of a specific object.The position returned is in worldspace coordinates for an actor or a component and screenspace coordinates for widgets. 

**Parameters**: 

  * **HPath** The HierarchyPath of the object to return the position of.
  * **coordinateSpace** The coorindate space conversion to perform on the position before returning it. See gdio.common.objects.CoordinateConversion for more information.
  * **valid** out param set to true if the HPath resolves and the call is possible.


**Return**: The Vector3 position of the specific object.





```cpp
 bool wasValid = false;
 FVector pos = UGDIOApi::GetObjectPosition("//ThirdPersonCharacter_167", CoordinateConversion::Local, wasValid);
    if (wasValid) {
    UE_LOG(LogTemp, Display, TEXT("%f %f %f"), pos.X, pos.Y, pos.Z);
}
```


### function GetObjectPosition

```cpp
static FVector GetObjectPosition(
    UObject * obj,
    CoordinateConversion coordinateSpace,
    bool & valid
)
```

Return the position of a specific object.The position returned is in worldspace coordinates for an actor or a component and screenspace coordinates for widgets. 

**Parameters**: 

  * **HPath** The HierarchyPath of the object to return the position of.
  * **coordinateSpace** The coorindate space conversion to perform on the position before returning it. See gdio.common.objects.CoordinateConversion for more information.
  * **valid** out param set to true if the HPath resolves and the call is possible.


**Return**: The Vector3 position of the specific object.





```cpp
 bool wasValid = false;
 //UObject* object is defined and assigned somewhere....
 FVector pos = UGDIOApi::GetObjectPosition(object, CoordinateConversion::Local, wasValid);
    if (wasValid) {
    UE_LOG(LogTemp, Display, TEXT("%f %f %f"), pos.X, pos.Y, pos.Z);
}
```


### function FloatInputEvent

```cpp
static bool FloatInputEvent(
    FKey key,
    double value
)
```

Use this function to simulate a KeyAxis float input (axis). Pass 0 to stop sending the event. 

**Parameters**: 

  * **key** The FKey that you want to iput a value for
  * **key** The Value you want to inject






```cpp
UGDIOApiUGDIOApi::FloatInputEvent("OculusTouch_Right_Thumbstick_Y", 0.75f);
//wait
UGDIOApiUGDIOApi::FloatInputEvent("OculusTouch_Right_Thumbstick_Y", 0f);
```


-------------------------------

Updated on 2023-12-12 at 14:22:15 -0700