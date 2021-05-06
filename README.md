# About
#### The 3DS version of Majora's Mask has terrible amounts of reverb; compared to the original soundtrack, a lot of the songs just sound wrong. I set out to fix this by replacing the 3DS OST with N64 rips. 
### Complimentary Mods:
### [Project Restoration](https://github.com/leoetlino/project-restoration) by [leoetlino](https://github.com/leoetlino) (Recommended)
### [MM3DHD](https://https://github.com/DeathWrench/MM3DHD) (WIP)
### Want something Different than the original OST?
### [Majora's Mask 3D Remastered Soundtrack](https://github.com/sygemdev/Majora-s-Mask-3D-Remastered-OST)
_____
### Optional [Keaton's Quiz](https://www.youtube.com/watch?v=Gi73mO54SBo) song replacer
* ### Midna's Lament by [Nerrel](https://www.patreon.com/Nerrel)
# [Download releases here](https://github.com/DeathWrench/Majora-s-Mask-N64-OST-to-3DS/releases/)

# Installation

## Luma:
* Hold Select while booting your 3DS and enable game patching in the Luma configuration menu.
* On your SD card, put the RomFS folder into luma/titles/0004000000125***X***00
* USA = 0004000000125***5***00
* EUR = 0004000000125***6***00
* Insert your SD card, restart the system, and changes should take place when you launch the game!
## Citra new method:
* Put the romfs folder in "%AppData%\Citra\load\mods\0004000000125X00" (by default) to apply the mod on Citra Canary
## Citra old method:
* Download the [3DS .NET Toolkit](https://github.com/evandixon/DotNet3dsToolkit/releases/) and use it to extract your Decrypted CCI/.3DS/.CIA ROM of the game. 
* Replace the files in the extracted RomFS directory with the ones from the .zip and rebuild the .3DS/.CIA file. 
* Then you can run/install it in Citra.

# Songs that can't be replaced 
The shop music, boat ride, milk bar, and minigame music are mono and sound like they're playing out of a radio. For some reason unbeknownst to me. Porting the originals causes extreme audio bugs and sometimes crashes, even when converted to mono.
If anyone can solve this mystery, I'll try and put them back in.

"130NA_BGM_STAFFROLL2.dspadpcm.wav" and "130NA_BGM_STAFFROLL2.dspadpcm_1.wav" can't be replaced because they're not in the original rips.

"NA_BGM_M_BARQUARTET.wav" While I can replace this, it didn't sound very good as I had to cut the entire song off half way, it sounded bad to me so I didn't do it.
####
The rest are just sound effects.

# Tools used
* [Audacity](https://www.audacityteam.org)
* [Fl Studio](https://www.image-line.com/flstudio)
* [Foobar2000](https://www.foobar2000.org)
* [Looping Audio Converter](https://github.com/libertyernie/LoopingAudioConverter/releases)
* my ears

# Playback
If you want to play these files back you need Foobar2000 and [vgmstream decoder](https://www.foobar2000.org/components/view/foo_input_vgmstream)

# Editing process
My process for editing the files in v2.0 went as follows:
#### Pre edits:
* Convert 3DS .bcstm files to .wav using foobar and place them in a folder called 3dswav
* Convert .miniusf rips to .wav using foobar and place them in a folder called 64wav
* Open Audacity and drag all the 64wav files into it
* CTRL + A to select all and change tempo to 6.1 to match the speed of the 3DS rip.
* Export multiple into a folder called 64sped
#### Edit edits:
* drag single 3DSwav file followed by the matching 64sped file
* Check hh:mm:ss + miliseconds to find the exact time of the miniusf rip now that it's sped up.
* Open the slow 64wav rip in FL Studio and normalize if the waveform is too small
* Time stretch / pitch shifter then put length as exact miliseconds
* Export
* Drag this new rip into the same Audacity window as before.
* Find loop points (if there are any) and put them into loop.txt
* If anything clips fix it
* Click the [x]s on the other rips and leave only this new edited rip
* Export at 32000hz .wav with metadata removed and then convert to .bcstm using Looping Audio Converter.
# Because of this process I am not completely satisfied with it, I require higher quality rips. If you send me these files. I will redo this mod a final time.

# How this came to be
I recently made an [MSU-1 pack for A Link to the Past](https://www.zeldix.net/t791-the-legend-of-zelda-a-link-to-the-past) with help from [qwertymodo](https://github.com/qwertymodo) converting the original soundtrack from ALTTP to .pcm in order to fix the music from cutting out when multiple sounds are playing. I was under the assumption that the 3DS version of Majora's Mask used sequenced audio for music. [Bl4zerp](https://github.com/bl4zerp) told me I was wrong so I looked into it. Turns out Majora's Mask music is in .bcstm format, which is basically .pcm, and now we're here.
