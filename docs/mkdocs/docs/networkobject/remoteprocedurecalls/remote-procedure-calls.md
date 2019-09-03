# Remote Procedure Calls

Remote procedure calls \(RPC\) is a way to call functions over the network. So lets imagine that you \(**ClientA**\) had a method named **"Explode"** and I \(**ClientB**\) wanted to call that **"Explode"** method on your machine so that we both see the fireworks at the same time. Your main question might be:

> "Well how can I call that function so that we both can see the fireworks explode at the same time?"

The answer of course is by doing a Remote Procedure call. An RPC can be called on a specific client, all clients, buffered clients, etc. RPCs use a reliable protocol - They always come in the right order and reception of RPCs is confirmed. To get you quickly started, check out the [Basic RPC Example](https://github.com/andreivreja/ForgeNetworkingRemastered/tree/3e106b6d53966d4ac3b3490b277edc6696d12aeb/GettingStarted/basic-rpc-example.md). Once you have gone through that example and consumed all of its educational value, feel free to brows the below links for more information.

* [Buffered RPCs](https://github.com/andreivreja/ForgeNetworkingRemastered/tree/3e106b6d53966d4ac3b3490b277edc6696d12aeb/docs/mkdocs/docs/NetworkObject/RemoteProcedureCalls/buffered-rpcs/README.md)
* [Sending RPC To Single Player](https://github.com/andreivreja/ForgeNetworkingRemastered/tree/3e106b6d53966d4ac3b3490b277edc6696d12aeb/docs/mkdocs/docs/NetworkObject/RemoteProcedureCalls/sending-rpc-to-a-single-player/README.md)
* [RpcArgs and RpcInfo Structs](https://github.com/andreivreja/ForgeNetworkingRemastered/tree/3e106b6d53966d4ac3b3490b277edc6696d12aeb/docs/mkdocs/docs/NetworkObject/RemoteProcedureCalls/rpcargs-and-rpcinfo-structs/README.md)
* [RPC Validation by Server](https://github.com/andreivreja/ForgeNetworkingRemastered/tree/3e106b6d53966d4ac3b3490b277edc6696d12aeb/docs/mkdocs/docs/NetworkObject/RemoteProcedureCalls/rpc-validation-by-server/README.md)
* [Replacing Previous Buffered RPCs](https://github.com/andreivreja/ForgeNetworkingRemastered/tree/3e106b6d53966d4ac3b3490b277edc6696d12aeb/docs/mkdocs/docs/NetworkObject/RemoteProcedureCalls/replacing-previous-buffered-rpcs/README.md)
* [Clearing Buffered RPCs](https://github.com/andreivreja/ForgeNetworkingRemastered/tree/3e106b6d53966d4ac3b3490b277edc6696d12aeb/docs/mkdocs/docs/NetworkObject/RemoteProcedureCalls/clearing-buffered-rpcs/README.md)

