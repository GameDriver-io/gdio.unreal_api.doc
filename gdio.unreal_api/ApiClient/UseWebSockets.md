# ApiClient.UseWebSockets method

Configure a WebSocket server for a client (GDIOAgent) to connect to.

```csharp
public void UseWebSockets(string hostname, int port, bool waitForAgentConnection = true, 
    int timeout = 60)
```

| parameter | description |
| --- | --- |
| hostname |  |
| port |  |
| waitForAgentConnection |  |
| timeout |  |

## Examples

```csharp
 //Waits for an inbound connection on localhost port 7072 for 120s.
            var task = new Task(() => api.UseWebSockets(testHost, 7072, true, 120));
            task.Start();
```

## See Also

* class [ApiClient](../ApiClient.md)
* namespace [gdio.unreal_api](../../gdio.unreal_api.md)

<!-- DO NOT EDIT: generated by xmldocmd for gdio.unreal_api.dll -->