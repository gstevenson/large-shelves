# Taller Shelves

A RimWorld mod that adds two new storage buildings — **Tall Shelf** (2x1) and
**Tall Shelf (small)** (1x1) — taller, reinforced versions of the vanilla
shelves that hold **twice as much per cell** (6 stacks vs. vanilla's 3).

Unlocked by a new research project, **Taller Shelving**, which requires
Complex Furniture (the same prerequisite as vanilla shelves).

This is a pure XML mod — no C# assembly, no Harmony patches, and vanilla
shelves are untouched. Safe to add to or remove from an existing save.

## Requirements

- RimWorld 1.6

## Installing from source (for development)

1. Clone this repo somewhere convenient, e.g. `C:\Projects\rimworld\large-shelves`.
2. Symlink it into RimWorld's local `Mods` folder so the game picks up edits
   live, instead of copying files back and forth. In an elevated PowerShell:

   ```powershell
   New-Item -ItemType SymbolicLink `
     -Path "<path-to-RimWorld>\Mods\TallerShelves" `
     -Target "C:\Projects\rimworld\large-shelves"
   ```

   Replace `<path-to-RimWorld>` with your install, e.g.
   `D:\Steam\steamapps\common\RimWorld`.
3. Launch RimWorld, open **Options → enable Developer mode** (this surfaces
   any XML load errors in the debug log).
4. From the main menu, open **Mods**, enable "Taller Shelves", and restart
   when prompted.
5. Start or load a game. Research **Taller Shelving**, then check the
   Furniture build menu for **Tall Shelf** / **Tall Shelf (small)**.

## Installing as a player (once published)

Subscribe on the Steam Workshop (link TBD) and enable it in the in-game Mods
menu — no manual steps needed.

## Mod structure

```
About/
  About.xml                          # mod metadata
Defs/
  ResearchProjectDefs/
    TallerShelving.xml               # the unlocking research project
  ThingDefs_Buildings/
    TallerShelves.xml                # the two shelf buildings
```

## License

TBD.
