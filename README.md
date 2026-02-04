# NatroMacroAddon

This repository is an addon fork of **Natro Macro**.

It currently includes improvements around **Bloom farming** and **Bloom-related quests** (e.g. Bucko/Riley/Polar “Bloom” objectives), and it is intended to grow with more features over time.

## ✨ Features

- __Bloom farming__: in every cycle it collects petals on the selected field for the set duration.
- __Bloom quests__: supports quests that require collecting bloom petals.

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

	<table style="border:none;border-collapse:collapse;border-spacing:0;">
		<tr>
			<td style="border:none;padding:0;"><span style="padding-right:10px;font-size:0.6em;">&#9675;</span><code>None</code></td>
			<td style="border:none;padding:0 0 0 10px;"><em>no checkbox enabled</em></td>
		</tr>
		<tr>
			<td style="border:none;padding:0;"><span style="padding-right:10px;font-size:0.6em;">&#9675;</span><code>Sprinkler on bloom</code></td>
			<td style="border:none;padding:0 0 0 10px;"><em>places the sprinkler down on each bloom</em></td>
		</tr>
		<tr>
			<td style="border:none;padding:0;"><span style="padding-right:10px;font-size:0.6em;">&#9675;</span><code>Sprinkler on field</code></td>
			<td style="border:none;padding:0 0 0 10px;"><em>places the sprinkler down upon arrival at the field</em></td>
		</tr>
	</table>

___The sprinkler settings also apply during bloom quests___

### Bloom Quest
> These settings only apply during bloom quests

- Set the maximum duration limit in the `Max Mins` textbox
- Set the fields for each petal color with the `"Color" Petal` dropdowns

___The ___

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
A screen limit has been set for closely neighboring fields, beyond which blooms are not detected, to prevent moving to other fields.<br/>
In some cases, this may cause blooms that are technically within the correct field but outside the limit to go undetected. <br/>
This issue has been resolved in certain fields; however, it does not work when fog is present, so the limit remains in place. <br/>
As a result, alignment moves the player to a position within the field where the majority of blooms can be detected.

### Misdetection

Balloons use the same icon that the macro searches for when detecting blooms. As a result, balloons may occasionally be misdetected as blooms. <br/>
The frequency of this issue has been reduced, but it can still occur. This does not significantly affect bloom farming, <br/>
as the macro typically misdetects it only once or twice before continuing to collect petals. <br/>
However, in rare cases, this may cause drifting off the field, and no reliable solution is currently available. <br/>
Puffshrooms also use the same icon; however, this issue does not occur with them.

### Early Stage

Bloom farming has been tested on both main and beginner profiles, as well as across multiple screen resolutions, and it seems to work in all cases. <br/>
However, this does not guarantee that it will work for everyone 100% of the time. This project is still in a very early stage and is not as polished as Natro Macro. <br/>
If major issues occur, efforts will be made to resolve them when possible.

## ©️ Credits / License

This project is a fork of **Natro Macro**.

- Upstream repository: https://github.com/NatroTeam/NatroMacro
- License: see `LICENSE.md` in this repository