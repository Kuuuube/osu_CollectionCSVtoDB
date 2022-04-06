# osu! CollectionCSVtoDB

Accepts CSV files with MD5 in the first column or any file with a newline separated MD5 list and converts to an osu! collection.

## Downloads

Downloads are available in [Releases](https://github.com/Kuuuube/osu_CollectionCSVtoDB/releases).

## Usage

Either run with or without command line args.

## Command line args:

```
CollectionCSVtoDB {input} {output}
```
## Dependencies

.Net Runtime 6.0 x64: https://dotnet.microsoft.com/en-us/download/dotnet/6.0

## Building:

Run `build.ps1` or manually run:

```
$options= @('--configuration', 'Release', '-p:PublishSingleFile=true', '-p:DebugType=embedded', '--self-contained', 'false')
dotnet publish CollectionCSVtoDB $options --runtime win-x64 --framework net6.0 -o build/win-x64
dotnet publish CollectionCSVtoDB $options --runtime linux-x64 --framework net6.0 -o build/linux-x64
```