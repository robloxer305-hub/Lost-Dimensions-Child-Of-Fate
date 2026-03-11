# RPGGame (C# + raylib-cs)

## Requirements
- Windows 10/11 x64
- .NET SDK installed

## Run (dev)
```powershell
dotnet run --project .\RPGGame.Client\RPGGame.Client.csproj
```

## Publish single-file .exe (Release)
```powershell
dotnet publish .\RPGGame.Client\RPGGame.Client.csproj -c Release -r win-x64 \
  /p:PublishSingleFile=true /p:SelfContained=true
```
Output:
- `RPGGame.Client\bin\Release\net10.0\win-x64\publish\RPGGame.Client.exe`

## Content
Data-driven content lives in `content/`:
- `content/items/items.json`
- `content/enemies/enemies.json`
- `content/quests/quests.json`
- `content/spawns/spawns.json`
- `content/settings.json`

Assets live in `assets/` and can be swapped without code changes.
