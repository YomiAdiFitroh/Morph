# Morph

**Drag. Drop. Converted.** A small, free file converter you use by dragging: hold a key (**Ctrl**, **Option** on macOS), drag files, and drop them on a format in the donut that opens at your cursor. Everything stays on your computer.

> Morph is a rebranded, lightened build of [Filee](https://github.com/KnifeLemon/Filee) by KnifeLemon, used under the MIT License (see [LICENSE](LICENSE)).

## What is different from Filee

- New name, icon and teal/amber colour palette; cleaner, cooler light surfaces and slightly tighter corners.
- Light theme by default (System and Dark are still in Settings → Theme).
- Lighter by default: no start with the system, no update checks against the original project, no feedback or sponsor prompts.
- Leaner runtime: no background-GC thread, no PGO instrumentation, more eager memory compaction, memory trimmed 10 s after the last conversion.

## Build and run (Windows)

1. Install the **.NET 10 SDK** (`global.json` pins 10.0.100).
2. From this folder:

```powershell
dotnet build src/Filee.App
dotnet run --project src/Filee.App
```

The program and its project files still use the internal name `Filee` (assembly `Filee.exe`, settings folder `%APPDATA%\Filee`); only what you see is Morph.

See `docs/ARCHITECTURE.md` and `docs/ADDING-A-CONVERTER.md` for how the code is organised.
