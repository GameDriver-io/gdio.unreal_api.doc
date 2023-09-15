# ApiClient.RemoveInputDevices method

Use this function to remove all GameDriver virtual VR devices

```csharp
public void RemoveInputDevices(int timeout = 30)
```

| parameter | description |
| --- | --- |
| timeout | The amount of time in seconds to wait for connectivity to establish with the game. |

## Examples

```csharp
// Removes all devices and layouts created by the GameDriver api
            api.RemoveInputDevices();
```

## See Also

* class [ApiClient](../ApiClient.md)
* namespace [gdio.unreal_api](../../gdio.unreal_api.md)

<!-- DO NOT EDIT: generated by xmldocmd for gdio.unreal_api.dll -->