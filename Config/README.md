# LDBTool

Library that allows mods to add and edit Proto data. Also allows you to see Proto data, config ID's of mod Protos and change localized strings

# List of features
- Add new Protos to game ProtoSets
- Edit existing Protos
- Configure ID, Grid index of created Protos in config file located at `Dyson Sphere Program/BepInEx/config/LDBTool`
- Customize mod localization
- View all Protos and inspect them using [UnityExplorer](https://dsp.thunderstore.io/package/sinai-dev/UnityExplorer/)

## Installation
### With Mod Manager

Simply open the mod manager (if you don't have it install it [here](https://dsp.thunderstore.io/package/ebkr/r2modman/)), select **LDB Tool by xiaoye97**, then **Download**.

If prompted to download with dependencies, select `Yes`.

Then just click **Start modded**, and the game will run with the mod installed.

### Manually
Install BepInEx from [here](https://dsp.thunderstore.io/package/xiaoye97/BepInEx/)<br/>
Unzip mod arhive into `Dyson Sphere Program/BepInEx/plugins/LDBTool/`. (Create folder named `LDBTool`)<br/>

## Development

### Creating a Release

This project uses GitHub Actions to automatically build and release packages. To create a new release:

1. Update the version number in `LDBTool/LDBToolPlugin.cs` (update the `VERSION` constant)
2. Update `Config/CHANGELOG.md` with the changes for the new version
3. Commit and push your changes to the main branch
4. Create and push a new git tag matching the version:
   ```bash
   git tag v3.0.3
   git push origin v3.0.3
   ```
5. The GitHub Actions workflow will automatically:
   - Build the .NET solution
   - Package the mod using the Thunderstore CLI
   - Create a GitHub release with the packaged .zip file

The release will be available on the [Releases page](https://github.com/rudedude693/DSP_LDBTool/releases).

## Feedback and Bug Report
Feel free to contact me via Discord (Kremnev8#3756) for any feedback, bug-reports or suggestions.