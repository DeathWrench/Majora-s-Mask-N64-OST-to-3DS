# About
#### The 3DS version of Majora's Mask has terrible amounts of reverb; compared to the original soundtrack, a lot of the songs just sound wrong. I set out to fix this by replacing the 3DS OST with N64 rips. 
### This also works with [Project Restoration](https://github.com/leoetlino/project-restoration)

# [Download releases here](https://github.com/DeathWrench/Majora-s-Mask-N64-OST-to-3DS/releases/)

# Installation

## Luma:
* Luma Instructions Hold Select while booting your 3DS and enable game patching in the Luma configuration menu.
* On your SD card, merge the luma folder (and its contents) from the ZIP with your luma folder.
* If your copy of the game is a different region, change the directory name inside \luma\titles to the [titleid of your copy.](https://titledb.com/) (e.g. 0004000000125500)
* Insert your SD card, restart the system, and changes should take place when you launch the game!

## Citra:
* Download the [3DS .NET Toolkit](https://github.com/evandixon/DotNet3dsToolkit/releases/) and use it to extract your Decrypted CCI/.3DS/.CIA ROM of the game. 
* Replace the files in the extracted Romfs directory with the ones from the zip and rebuild the .3DS/.CIA file. 
* Then you can run/install it in Citra.

# Songs that can't be replaced. 
The shop music, boat ride, milk bar, and minigame music are mono and sound like they're playing out of a radio. For some reason unbeknownst to me. Porting the originals causes extreme audio bugs and crashes even when converted to mono.
If anyone can solve this mystery, I'll try and put them back in.

# Tools used
* [Fl Studio](https://www.image-line.com/flstudio)
* [Audacity](https://www.audacityteam.org)
* [Looping Audio Converter](https://github.com/libertyernie/LoopingAudioConverter/releases)
* my ears

# How this came to be
I recently made an [MSU-1 pack for A Link to the Past](https://www.zeldix.net/t791-the-legend-of-zelda-a-link-to-the-past) with help from [qwertymodo](https://github.com/qwertymodo) converting the original soundtrack from ALTTP to .pcm in order to fix the music from cutting out when multiple sounds are playing. I was under the assumption that the 3DS version of Majora's Mask used sequenced audio for music. Bl4zerp told me I was wrong so I looked into it. Turns out Majora's Mask music is in .bcstm format, which is basically .pcm, and now we're here.
