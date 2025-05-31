# Stellaris Checksum Patcher

## 📣 Summary
An easy and painless way to patch the game's executable so that mods which change the checksum can still allow achievements to be earned.

<p align="center">
<img src="https://github.com/r0fld4nc3/stellaris-exe-checksum-patcher/blob/main/media/stellaris-checksum-patcher-06.png" width="762">
</p>

## ❗ Disclaimer ❗
* Remember to **not** upload the modified Stellaris executable to download or distribution sites. My stance on this is further down.
* Use at your own risk. I take no responsibility for your actions or what you choose to do with the modified file.
* The goal of this is to simply offer a faster and more automated way to enable mod compatibility with achievements for a better personal experience.
* Check notes at the end of this file on how to build the code, contributions are welcome!

## 🟢 Features:
* **Patch Executable**
  * This method will automatically check for a Steam installation and patch the executable.
  * It will create a backup of the original adding a _.orig_ to the end of the file name.
  * If it cannot find the installation, will prompt via dialog for the install folder.
  * Will remember the installation location for next time.

* **Fix Save Achievements**
  * Will ask for the save file to work on
  * Attempts to fix achievements not being present.
  * Sets Ironman flag(s) to "yes".

# 🗒️ Notes
The cause of the issue where after an update, achievements were no longer being triggered has been identified. 
The issue is with game updates and save games, where sometimes saves can lose their trait of being eligible for achievements across patches.
I will be working on a "Fix Save Game" patch option as well to include in the Patcher in the future, to fix this issue.

❗ Save fixing not yet done for Windows, MacOS and Linux.


# 🔎 My Stance
The sole reason for this patch comes mostly for the fact that we are barred from amazing Quality of Life and Visual mods if we wish to hunt for those Achievements.

I don't wish to make it so that it becomes easier or _cheesier_ or _cheatier_ to acquire those Achievements as personally that would also completely devalue the effort made. I do support there being no access to the console or any other way to circumvent certain aspects that deter from the challenge, and I understand how difficult or nearly impossible it is to dynamically regulate which mods would be valid and which ones would not.

**Therefore, I do not condone and do not support bypassing this restriction by the developers with the aim of installing content that would enable cheating or unfairly facilitate the acquisition of Achievements, nor was this application made with that belief in mind.**

I understand I cannot regulate this either and therefore ask for sensibility and fairness when playing with the patch in place. These achievements and everything surrounding them were done with great care and passion by fellow people and it is our responsibility to care for and respect their creations which they poured their hearts and hours into.

## Sources
This method was a side project mainly for learning purposes and honing skills. _(Also because I don't have MSWord lol)_

It was based on an original guide here: https://steamcommunity.com/sharedfiles/filedetails/?id=2719382752.

and forked from https://github.com/r0fld4nc3/Stellaris-Exe-Checksum-Patcher by `TheCosmicSlug` when the v4.0 Stellaris update released.

previously had been using Ghidra and the guide at: https://steamcommunity.com/sharedfiles/filedetails/?id=2460079052

I build this version using Ubuntu linux and VScode. For instructions how to setup an environment goto:
https://github.com/thecosmicslug/Stellaris-Checksum-Patcher/blob/main/BUILDING.MD
