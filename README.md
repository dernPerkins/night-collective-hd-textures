# Night Society HD Textures

Optional HD texture packs for **Night Society**, the native PC and Android
port of *Midnight Club 3: DUB Edition Remix*.

The packs are downloaded from inside the game. Nothing here runs on its own,
and nothing here is the game: you still need your own copy of the disc.

## Packs

| Pack | Covers | PC (DDS, BC7) | Android (KTX2, ASTC 4x4) |
|---|---|---|---|
| UltraSharp 2x full | every texture on the disc: all four cities, every time of day and weather, every car, the menus and the HUD | 742 MB | 743 MB |

Each texture is upscaled 2x with the
[UltraSharp V2](https://huggingface.co/Kim2091/UltraSharpV2) model by Kim2091
(CC BY-NC-SA 4.0). The packs are free and non-commercial, and that credit is
given here. They are built with the game's `tools/texpack/texpack.py` from
the textures on the disc, so they match the game's own texture names
exactly.

## Installing

**In the game (recommended):** open the settings (F1 on PC, Back+Start on a
controller), go to **Graphics**, and pick **Download UltraSharp 2x full**
under **HD textures**.

- The pack unpacks as it downloads, so it never takes up the space twice.
- If the download stops or the connection drops, it carries on from where it
  got to next time.
- When it finishes, it is switched on.

**By hand:** download the zip for your platform from the
[latest release](../../releases/latest) and unzip it into the game's
`texpacks` folder, so you end up with `texpacks/UltraSharp 2x full/pack.toml`.
Then pick it under **Graphics → HD textures**.

| Platform | `texpacks` folder |
|---|---|
| PC | next to the game's `game` folder |
| Android | `Android/data/io.github.mc3x.recomp/files/texpacks/` |

## Turning it off

**Graphics → HD textures → Off** puts the game's original textures back at
once. Delete the pack's folder to free the space.

## The release files

Each release holds:

- `ultrasharp-2x-full-desktop.zip`: `pack.toml` and the DDS pictures, for PC
  GPUs.
- `ultrasharp-2x-full-android.zip`: `pack.toml` and the KTX2 pictures, for
  phones and handhelds.
- `packs.tsv`: the catalog the game reads (title, folder, platform, size,
  address of each zip).

The zips are stored, not compressed. That is what lets the game unpack them
while they download, and the pictures are already compressed GPU formats
that would barely shrink anyway.

## Legal

*Midnight Club 3: DUB Edition Remix* and its artwork belong to Rockstar
Games and Take-Two Interactive. These packs are upscaled derivatives of that
artwork, offered for players who own the game. This project is not
affiliated with or endorsed by Rockstar Games or Take-Two Interactive.

The upscaling model, UltraSharp V2 by Kim2091, is licensed CC BY-NC-SA 4.0.
These packs are distributed free of charge and must not be sold.
