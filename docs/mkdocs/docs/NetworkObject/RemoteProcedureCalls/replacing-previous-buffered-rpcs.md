# Replacing Previous Buffered RPCs

There are times where the buffered data that you want to send to new players that connect needs to be updated. Let's say that you were sending the current color of the winning team to a connecting player. Though you could run this on [playerAccepted](https://github.com/andreivreja/ForgeNetworkingRemastered/tree/3e106b6d53966d4ac3b3490b277edc6696d12aeb/connection-cycle-events.md#playerAccepted) you might choose to do this with a buffered RPC.

Unfortunately the currently winning team may change and so the color would need to be buffered yet again. If you were to keep buffering the team color you may end up with a buffer of 50 RPCs, so all 50 would get sent in order to the connecting player. Instead you can choose to replace the last call to a buffered RPC which will remove the last RPC called on **this specific** game object with the given RPC string name with the one you are currently executing. This is done easily by passing **true** to the `SendRpc` method overload that has the **replacePrevious** argument:

```csharp
bool replacePrevious = true;
networkObject.SendRpc(RPC_MY_RPC_NAME, replacePrevious, Receivers.AllBuffered, new object[] { "args go here" });
```

