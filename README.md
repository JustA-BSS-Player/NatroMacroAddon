# NatroMacroAddon

This repository is an addon fork of **Natro Macro**.

It currently includes improvements around **Bloom farming** and **Bloom-related quests** (e.g. Bucko/Riley/Polar “Bloom” objectives), and it is intended to grow with more features over time.

## ✨ Features

- __Bloom farming__: in every cycle it collects petals on the selected field for the set duration.
- __Bloom quests__: supports quests that require collecting bloom petals.

## ▶️ YouTube
__Check out my YouTube channel for tutorials and showcases:__

[![YouTube](https://img.shields.io/badge/Watch%20on-YouTube-red?logo=youtube)](https://www.youtube.com/@JustA-BSS-Player)

## 🛠️ Installation
_Basically the same as `Natro Macro`_

1. Download/clone this repository
2. Open `NatroMacroAddon` and double-click the folder inside
3. Run `START.bat` and wait for the macro to load

## ⚙️ Usage

### Bloom
>These settings only apply during the gather cycle bloom farming

- Enable it with the `✅Enable` checkbox next to the __Bloom__ text
- Set the field with the `Field` dropdown
- Set the duration in the `Mins` textbox
- Set the `To Hive By` method with the arrows
- Set the sprinkler placement method:
	- `None`: _no checkbox enabled_
	- `Sprinkler on bloom`: _places the sprinkler down on each bloom_
	- `Sprinkler on field`: _places the sprinkler down upon arrival at the field_

___The sprinkler settings also apply during bloom quests___

### Bloom Quest
> These settings only apply during bloom quests

- Set the maximum duration limit in the `Max Mins` textbox
- Set the fields for each petal color with the `"Color" Petal` dropdowns

___The fields are ordered based on how good they are for collecting that color___

<br/>
Bloom quest handling is implemented for:

- **Polar Bear** quests
- **Gifted Riley Bee** quests
- **Gifted Bucko Bee** quests

## ⚠️ Limitations / Known Issues

### Missing fields
__No reliable alignment pattern:__
- Mountain Top field
- Stump field

__Too many obstacles on the field:__
- Mushroom field

### Field limit
A screen limit has been set for closely neighboring fields, beyond which blooms are not detected, to prevent moving to other fields. In some cases, this may cause blooms that are technically within the correct field but outside the limit to go undetected. This issue has been resolved in certain fields; however, it does not work when fog is present, so the limit remains in place. As a result, alignment moves the player to a position within the field where the majority of blooms can be detected.

### Misdetection

Balloons use the same icon that the macro searches for when detecting blooms. As a result, balloons may occasionally be misdetected as blooms. The frequency of this issue has been reduced, but it can still occur. This does not significantly affect bloom farming, as the macro typically misdetects it only once or twice before continuing to collect petals. However, in rare cases, this may cause drifting off the field, and no reliable solution is currently available. Puffshrooms also use the same icon; however, this issue does not occur with them.

### Early Stage

Bloom farming has been tested on both main and beginner profiles, as well as across multiple screen resolutions, and it seems to work in all cases. However, this does not guarantee that it will work for everyone 100% of the time. This project is still in a very early stage and is not as polished as Natro Macro. If major issues occur, efforts will be made to resolve them when possible.

## ©️ Credits / License

This project is a fork of **Natro Macro**.

- Upstream repository: https://github.com/NatroTeam/NatroMacro
- License: see `LICENSE.md` in this repository