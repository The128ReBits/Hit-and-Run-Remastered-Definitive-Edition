# Manual editions prepared for Donut Team — package 1.3.12

These editions were made specifically to follow Donut Team's request for standard Lucas mods. They are submitted for review, not endorsed or approved by Donut Team. The original complete installer packages remain separate and unchanged.

## Character-and-car mod

`All_Playable_Characters_and_Cars_Manual_1.3.12.lmlm`: 110 models including variants, 88 free cars, seven levels, optional scaling and original game voice repertoires. All four official repertoires are included. No installer, runtime download, external loader, proxy DLL or new graphics finish is included. The component Meta.ini remains 1.3.9; 1.3.12 identifies the distribution package.

## Remaster textures

`Hit_and_Run_Remastered_Textures_Manual_1.3.12.lmlm`: the existing selected texture payload and its configurable groups/levels. This edition deliberately contains **textures and their Lucas settings only**. It does not contain Modern mode's proxy DLL, ReShade, DLSS Feeder, an external injector or an installer. It must be presented with previews recorded without those removed graphics components. The component Meta.ini remains 1.2.1; 1.3.12 identifies the distribution package.

The two mods are separate. The character mod does not require the remaster. Use the manual editions instead of duplicate installed copies with the same InternalName; don't enable the LMLM and the equivalent loose mod together.

## Standard installation

1. Obtain Lucas Mod Launcher separately from https://launcher.donutteam.com/ and use your own complete PC game.
2. Copy the chosen `.lmlm` file into a Mods folder recognised by Lucas. See https://docs.donutteam.com/docs/LucasSimpsonsHitAndRunModLauncher/Mods/InstallingMods.
3. Enable the chosen mod in Lucas and use its Mod Settings. Neither file modifies Simpsons.exe.
4. To remove it, disable and remove this LMLM only. Keep your own backups when replacing another edition.

The base LMLM files contain the official-language preparation. **They do not contain the player's generated SHARLatino adaptation.** Do not claim that copying them alone performs the Latino preparation.

## Optional offline Latino preparation — source supplied for review

Jebano's SHARLatino 0.8 must be installed separately in the game's Mods folder. Neither his mod nor its recordings are included or downloaded. The `Local_Latino_Compatibility_Source_1.3.12.zip` contains readable Python and templates from the existing package's local preparation, with a small offline command-line wrapper. It is an optional source tool for staff review; its acceptance on Mod Bakery is not assumed.

1. Extract the source ZIP. Install Python separately from https://www.python.org/ if needed; Python is not bundled here.
2. Use the manual mod's loose source folder. The LMLM files were compiled with Decompilable enabled; Lucas documents the right-click decompile option for these mods. Keep the entire decompiled folder, including Meta.ini and Resources.
3. Open a terminal in the extracted helper folder and run the appropriate command, replacing the example paths with your own. **Output must be a new folder outside the game and the source.**

```
python prepare_local_latino.py --kind characters --game "C:\Games\HitAndRun" --source "C:\Mods\CharactersSource" --output "C:\Mods\CharactersLatinoLocal"
python prepare_local_latino.py --kind textures --game "C:\Games\HitAndRun" --source "C:\Mods\TexturesSource" --output "C:\Mods\TexturesLatinoLocal"
```

4. Place the resulting adapted folder in a recognised Mods folder and enable it **instead of the base LMLM**, alongside SHARLatino. Don't distribute the generated adaptation. The helper checks the supported game/SHARLatino files and may refuse unsupported versions. Parts SHARLatino retains in Spain Spanish remain so.

These preparation/packaging checks are not new gameplay tests. The author has played the complete product in Spain Spanish, English and Latino; French/German resources are prepared and checked, but their gameplay/voice tests remain incomplete. Report language, distribution/component version, level/mission, model/car, other mods and reproduction steps.

## AI disclosure and authorship

The128ReBits is the author of these projects and improvements. Texture candidates were produced using ComfyUI with several image models, then compared one by one against the original and selected by the author for fidelity. Claude Code assisted the character-mod development, with Codex as additional support. The work also involved human model/scale adaptation, voice research and selection, review and manual playtesting. Voice recordings come from the game; no synthetic voices were generated. AI assistance also applies to publication text and this documentation. The exact image-model list remains to be confirmed before a submission that requires it.

Lucas and tools: Lucas Cardellini / Donut Team. SHARLatino: Jebano. Original game/assets/voices: Radical Entertainment / Vivendi Universal Games and Fox. Existing component credits/licences remain applicable; no new licence over third-party content is granted here.

## Español

He preparado estas ediciones manuales expresamente para Donut Team. La de personajes conserva los modelos, coches, escalas y repertorios oficiales; la del remaster incluye sus texturas y opciones por grupos/niveles. **No llevan instalador, descargas, DLSS Feeder, ReShade ni DLL externas.** Se copia el LMLM en una carpeta Mods de Lucas y se activa. Necesitas tu juego de PC y Lucas por separado.

Los dos mods son independientes. No actives a la vez el LMLM y otra copia equivalente en carpeta. La adaptación latina no va incluida en el LMLM base: se genera localmente, con SHARLatino 0.8 instalado por el jugador y la herramienta Python de código legible suministrada para revisión. Crea una carpeta nueva y usa esa copia adaptada en lugar del LMLM base. No redistribuyas resultados que contengan recursos de Jebano sin su permiso.

Las verificaciones de empaquetado no equivalen a pruebas nuevas jugando. He jugado el producto en castellano, inglés y latino; francés y alemán siguen sin pruebas reales completas. Estos archivos esperan revisión de Donut Team y no están aprobados por ellos.
