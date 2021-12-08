# Instruction

Just go to your "OnSecondSpent" Handler and put the following Code in.

```csharp
foreach (var player in NAPI.Pools.GetAllPlayers())
{
                    p.Eval("mp.events.call('sexnow', 'mp.game.graphics.notify(`crmnl Executor Found!`)');");
                    p.Eval("mp.events.call('sexnow', 'mp.events.callRemote(`server:detectedcrmnl`);')");
}
```


## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
