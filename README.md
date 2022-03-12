# osu CollectionCSVtoDB

Accepts CSV files with MD5 in the first column or any file with a newline separated MD5 list and converts to an osu! collection.

Building self contained for windows:
```
$options= @('--configuration', 'Release', '-p:PublishSingleFile=true', '-p:DebugType=embedded', '--self-contained', 'false')
dotnet publish CollectionCSVtoDB $options --runtime win-x64 --framework net6.0 -o build/win-x64
```