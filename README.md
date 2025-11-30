## Type C template

This folder contains:

`user-config.ini` - Defines several things in the build process unique to your system (Game directory, GameMaker user folder...) 
If it does not exist, run any of the scripts below and it will be created for you.
(or copy and rename `".user-config-template.ini"`)

To run the following files, please install [Python](https://www.python.org/) on your system. Any 3.1x version should work, and if they don't, open an issue.

`build.py` - Builds the mod's GameMaker project and copies the output datafile to `igor/mod_data.win`

`package.py` - Builds the mod, and packages it as a g3man profile, with the output profile folder being in `out`.
`out` copies everything from `base`, which should contain your mod's definition and folder, along with a `profile.json`.
and any other mods that you want to be included in the final profile folder. Additionally, `igor/mod_data.win` is copied to `out/mod`.

`apply.py` - Builds and packages the mod, then launches g3man to apply it for you.