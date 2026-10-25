# Customize+ (VierAI-fied)

> **Disclaimer:** this is an unofficial fork of Customize+. Its changes are AI-generated ("vibe coded"). It is not made, endorsed or supported by the Customize+ team, so please don't ask them for help with it. Use it at your own risk.

## Official Customize+

Links from the original README:

### <center>[FAQ](https://github.com/Aether-Tools/CustomizePlus/blob/main/docs/FAQ.md) | [Support Discord](https://discord.gg/KvGJCCnG8t) | [Contributing](https://github.com/Aether-Tools/CustomizePlus/blob/main/docs/CONTRIBUTING.md) | [Changelog for external tool developers](https://github.com/Aether-Tools/CustomizePlus/blob/main/docs/DEVELOPER_CHANGELOG.md)</center>

Add [Aether Tools](https://github.com/Aether-Tools/DalamudPlugins) or [Sea of Stars](https://github.com/Ottermandias/SeaOfStars) dalamud repository by following instructions on the respective pages. 

Original source: [Aether-Tools/CustomizePlus](https://github.com/Aether-Tools/CustomizePlus)

## What this fork changes

Full list: [CHANGELOG.md](CHANGELOG.md)

- **Skeleton swaps (testing build):** armatures rebuild when the skeleton is replaced, so temporary/IPC profiles reapply instead of half-applying.
- **Fixes:** temporary profiles no longer stop early; mount bones follow the actual rider; the mount-owner cache is pruned.
- **Performance:** allocation-free bone name matching, cached mount rider lookup, fewer per-frame allocations.

## Installing this fork

Add this custom plugin repository in Dalamud (`/xlsettings` > Experimental > Custom Plugin Repositories), then install it from `/xlplugins`:

`https://raw.githubusercontent.com/VierAI/DalamudPlugins/main/vierai.json`

## For the Customize+ team

If the original Customize+ authors would like any of these changes sent back upstream as pull requests, please open an issue on this repository or contact the fork maintainer, and we'll gladly prepare them.

## Licence and credits

This fork keeps the original licence, Apache License 2.0 (see [LICENSE.md](LICENSE.md)), and all original credits. See [MODIFICATIONS.md](MODIFICATIONS.md) for the list of changed files.

The original README follows unchanged.

---

## Original README

# Customize+
Customize+ is a Dalamud plugin designed to give you better control over your Final Fantasy XIV character appearance. Namely it allows you to apply character bone manipulations during gameplay.

### <center>[FAQ](https://github.com/Aether-Tools/CustomizePlus/blob/main/docs/FAQ.md) | [Support Discord](https://discord.gg/KvGJCCnG8t) | [Contributing](https://github.com/Aether-Tools/CustomizePlus/blob/main/docs/CONTRIBUTING.md) | [Changelog for external tool developers](https://github.com/Aether-Tools/CustomizePlus/blob/main/docs/DEVELOPER_CHANGELOG.md)</center>

## I need help with using Customize+!
Please check FAQ and, if needed, ask your question in support discord server run by our community: [Aetherworks](https://discord.gg/KvGJCCnG8t).

**Do not ask for help or support in issues section on GitHub.**

**Consult with community support team over at Discord before creating an issue in this repository.**

**Before reporting bug or leaving a suggestion in this GitHub you need to **carefully** read [issue creation guidelines](https://github.com/Aether-Tools/CustomizePlus/issues/11).**

## Installing
**Do not use repo.json from this repository**

Add [Aether Tools](https://github.com/Aether-Tools/DalamudPlugins) or [Sea of Stars](https://github.com/Ottermandias/SeaOfStars) dalamud repository by following instructions on the respective pages. 

Then search for Customize+ in the plugin manager.

## Development team
* [Risa](https://github.com/RisaDev/) - Customize+ 2.0 Author and Lead Developer.

## Acknowledgements
* User interface and general plugin architecture is heavily based on the code written as a part of [Glamourer](https://github.com/Ottermandias/Glamourer) project and supporting libraries. Original code is licensed under Apache License 2.0.
* Some of the game object interaction code is copied from [Penumbra](https://github.com/xivdev/Penumbra) and [Glamourer](https://github.com/Ottermandias/Glamourer) projects in order to make Customize+ not rely on Penumbra being installed.
* GitHub workflows have been taken from [Glamourer](https://github.com/Ottermandias/Glamourer) project.
* Customize+ is using code from [ECommons](https://github.com/NightmareXIV/ECommons) library for IPC functionality.
* Some of the bone manipulation code was taken from [Ktisis](https://github.com/ktisis-tools/Ktisis).
* Thanks to [Dalamud](https://github.com/goatcorp/Dalamud) team for making plugins possible at all.
* Special thanks goes to Yuki, Phenrei, Stoia, dendr01d and others for developing and maintaining original (1.0) version of Customize+.
* Thank you to everyone who contributed new features and bug fixes through pull requests.

## License
All files in this repository are licensed under the license listed in LICENSE.md file unless stated otherwise. By contributing the code into this repository you agreeing with licensing submitted code under this license.

*Customize+ includes code previously licensed to it by its contributors under MIT license. The text of the MIT license can be found [here](https://opensource.org/license/mit/). This code has been relicensed under license listed in LICENSE.md file.*

##### Final Fantasy XIV © SQUARE ENIX CO., LTD. All Rights Reserved. Customize+ and its developers are not affiliated with SQUARE ENIX CO., LTD. in any way.
