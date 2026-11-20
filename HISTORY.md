# History of Freeze Tag for TF2

Freeze Tag is a TF2 server mod based on the children's game: players who die freeze where they fell, and a teammate standing close enough thaws them out. Several SourceMod plugins have done this over the years. This repo carries **Friagram's** version.

Researched Nov 20, 2026 from the AlliedModders forums, the TF2 Wiki and copies of the code on GitHub. Links at the bottom.

## 2009: Chase's Freeze Tag (the first one)

- **[TF2] Freeze Tag** by **Chase**, posted on AlliedModders on Oct 12, 2009 (the source header says Oct 4, 2009). AlliedModders plugin ID 1219, last version 1.1.
- Frozen players waited for a teammate or a timer (`freezetag_autounfreeze`); it ran alongside normal game modes.
- Its source says "Portions adapted from Roll The Dice by linux_lover and TF2 Respawn by WoZer" and "Licensed under the GPL v2 or above".
- Later **unapproved** on AlliedModders (by psychonic) for "Very little feedback and requires the now-outdated duckhacks".
- The TF2 Wiki's Freeze Tag page still links to this plugin.

## 2012–2013: Friagram's Freeze Tag (this one)

- **[TF2] Freeze Tag** by **friagram**, AlliedModders plugin ID 3438, "Converts any map into a Freeze-Tag game mode". Contact in the code: http://steamcommunity.com/groups/poniponiponi.
- When players die they are encased in ice (the ice shard model in this repo). The author noted the model also lets players hide behind frozen teammates, which makes spies more useful.
- Version history from the forum thread:
  - **1.0.0**: Dec 30, 2012 (first post; tested on the TF2 beta with SourceMod 1.5 dev builds)
  - 1.0.2, then **1.0.6**: early Jan 2013 bug fixes
  - **1.0.7 beta**: Jan 8, 2013 (queued class changes, translation fixes, one-player rounds don't end)
  - **1.0.9**: Jan 14, 2013 (1.0.8 was internal; new config options for new play styles)
  - **1.1.0**: Jan 15, 2013 (fixed entities being killed wrongly, which removed weapons or crashed)
  - **1.1.4**: May 12, 2013, the last release
- Friagram's other TF2 plugins on AlliedModders include Third Person / Clientprefs and Gravestone Markers.
- Friagram's code is a separate plugin from Chase's (different author, structure and config). Whether it borrowed anything from Chase's is not stated anywhere I found.

## Others

- **Fluttershy's Freeze Tag** (austinwagner on GitHub), version 0.5.0: another independent take, needing TF2Items Give Weapon.
- Copies of Friagram's 1.1.4 also sit in other people's GitHub repos (e.g. Nopied/useless).

## 2026: this repo

By 2026, 1.1.4 no longer started rounds on current TF2 (spawn points now come back as negative entity references). This repo fixes that, makes TF2 bots ignore frozen players and keeps frozen players visible. See the README.

## License

- Chase's 2009 plugin: GPL v2 or later (stated in its source).
- Friagram's 1.1.4: **no license is stated** in the source file or in anything found so far. Until that's known, this repo has no license file, and the plugin remains Friagram's work.

## Sources

- AlliedModders: [[TF2] Freeze Tag by friagram (thread 204415)](https://forums.alliedmods.net/showthread.php?p=1863390), [archive view](https://forums.alliedmods.net/archive/index.php/t-204415.html)
- AlliedModders: [[TF2] Freeze Tag by Chase (thread 106248)](https://forums.alliedmods.net/showthread.php?t=106248)
- Chase's source: [MultipleEntendre/TF2-FreezeTag](https://github.com/MultipleEntendre/TF2-FreezeTag/blob/master/TF2_FreezeTag.sp)
- [SourceMod plugin list for Friagram](http://www.sourcemod.net/plugins.php?cat=0&mod=-1&author=Friagram&search=1)
- [TF2 Wiki: Freeze Tag](https://wiki.teamfortress.com/wiki/Freeze_Tag)
- [austinwagner/fluttershy_freezetag](https://github.com/austinwagner/fluttershy_freezetag)
