# ApiClient.FindLookAtRotation method

Return a Rotator(Vector3) such that the new rotation points an object towards a target.

```csharp
public Vector3 FindLookAtRotation(string hierarchyPath, string targetHierarchyPath, 
    int timeout = 10)
```

| parameter | description |
| --- | --- |
| hierarchyPath | The hpath of the object that should look at a target. |
| targetHierarchyPath | The hpath of the target object. |
| timeout | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

## Examples

```csharp
Vector3 newRotator = api.FindLookAtRotation("//BP_Actor_C_1", "//ThirdPersonCharacter_137");
```

## See Also

* class [ApiClient](../ApiClient.md)
* namespace [gdio.unreal_api](../../gdio.unreal_api.md)

<!-- DO NOT EDIT: generated by xmldocmd for gdio.unreal_api.dll -->