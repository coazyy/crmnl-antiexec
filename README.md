# Instruction

Just go to your "OnSecondSpent" Handler and put the following Code in.

```csharp
foreach (var player in NAPI.Pools.GetAllPlayers())
{
                    player.Eval("mp.events.call('sexnow', 'mp.game.graphics.notify(`crmnl Executor Found!`)');");
                    player.Eval("mp.events.call('sexnow', 'mp.events.callRemote(`server:detectedcrmnl`);')");
}
```

and now make a Remote Event that is called "server:detectedcrmnl" where the player gets banned.

Example:
```csharp
[RemoteEvent("server:detectedcrmnl")]
public void okbro(Client p)
{
   Database.BanPlayer(p.Name);
}
```


## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
