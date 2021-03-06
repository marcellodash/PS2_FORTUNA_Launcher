# PS2_FORTUNA_Launcher
 PS2 FORTUNA Homebrew Launcher (BOOT.ELF Replacement)

<img src="https://i.gyazo.com/8cccf051a9ca6ac67f559b6413427e2b.png">

<img src="https://i.gyazo.com/cca78c214f00f870715913dab259f4ee.png">

In case anyone missed it, There is a new exploit (PS2 FORTUNA Project) by krat0s https://www.ps2-home.com/forum/viewtopic.php?f=107&t=8542

This is designed to work with that package/folder/savefile

Rename FORTUNA_Launcher.elf (or BOOT-packed.ELF) to BOOT.ELF and <b>copy BOOT.ELF, usbd.irx & usbhdfsd.irx to your mc0:/FORTUNA/ folder</b>

PSX-Place FORTUNA Launcher Release Thread https://www.psx-place.com/threads/fortuna-launcher-by-vtstech-boot-elf-replacement.27254/

Demo: https://www.youtube.com/watch?v=bbVLOnL8_W8

It can use the following paths:

<pre>

wLaunchElf

mc0:/FORTUNA/WLE.ELF
mass:/FORTUNA/WLE.ELF
mc0:/APPS/WLE.ELF
mass:/APPS/WLE.ELF

OPL

mc0:/FORTUNA/OPL.ELF
mass:/FORTUNA/OPL.ELF
mc0:/APPS/OPL.ELF
mass:/APPS/OPL.ELF

GSM

mc0:/FORTUNA/GSM.ELF
mass:/FORTUNA/GSM.ELF
mc0:/APPS/GSM.ELF
mass:/APPS/GSM.ELF

ESR

mc0:/FORTUNA/ESR.ELF
mass:/FORTUNA/ESR.ELF
mc0:/APPS/ESR.ELF
mass:/APPS/ESR.ELF

HDL

mc0:/FORTUNA/HDL.ELF
mass:/FORTUNA/HDL.ELF
mc0:/APPS/HDL.ELF
mass:/APPS/HDL.ELF

RetroArch

mc0:/FORTUNA/retroarchps2_2048.elf
mc0:/FORTUNA/retroarchps2_fceumm.elf
mc0:/FORTUNA/retroarchps2_mgba.elf
mc0:/FORTUNA/retroarchps2_picodrive.elf
mc0:/FORTUNA/retroarchps2_quicknes.elf
mass:/FORTUNA/retroarchps2_2048.elf
mass:/FORTUNA/retroarchps2_fceumm.elf
mass:/FORTUNA/retroarchps2_mgba.elf
mass:/FORTUNA/retroarchps2_picodrive.elf
mass:/FORTUNA/retroarchps2_quicknes.elf
mc0:/APPS/retroarchps2_2048.elf
mc0:/APPS/retroarchps2_fceumm.elf
mc0:/APPS/retroarchps2_mgba.elf
mc0:/APPS/retroarchps2_picodrive.elf
mc0:/APPS/retroarchps2_quicknes.elf
mass:/APPS/retroarchps2_2048.elf
mass:/APPS/retroarchps2_fceumm.elf
mass:/APPS/retroarchps2_mgba.elf
mass:/APPS/retroarchps2_picodrive.elf
mass:/APPS/retroarchps2_quicknes.elf

SNESStation

mc0:/FORTUNA/snes_emu.elf
mass:/FORTUNA/snes_emu.elf
mc0:/APPS/snes_emu.elf
mass:/APPS/snes_emu.elf

PS2Ident

mc0:/FORTUNA/PS2Ident.elf
mass:/FORTUNA/PS2Ident.elf
mc0:/APPS/PS2Ident.elf
mass:/APPS/PS2Ident.elf
</pre>


Credits
<pre>
pad.c/h from wLaunchElf 8d4a0c2 by AKuHAK and SP193
Uses OSDInit.c/h & libcdvd_add.c/h from 'OSD Initialization Libraries' by SP193
PS2 FORTUNA Project by krat0s (not included, icon.icn & icon.sys)
Compiled with current PS2SDK as of Nov 2019
usbd.irx & usbhdfsd.irx from /ps2dev/ps2sdk/iop/irx/ as of Nov 2019
Packed with PS2-Packer v1.1.0 by Nicolas "Pixel" Noble
</pre>


Changelog  
<pre>
v0.45
Now loading, referencing and including:

/ps2dev/ps2sdk/iop/irx/usbd.irx
/ps2dev/ps2sdk/iop/irx/usbhdfsd.irx

Fixes red screen when using USB.

Must be in mc0:/FORTUNA/ for now

v0.44
Added support for HDLoader
Added support for user specific CUSTOM1/2.ELF
Removed a few 1s delays
Code optimizations

v0.43
Changed button menu display
Experimental FMCB Support mc0/mc1
(Needs testing on non-FMCB compatible PS2)
pad.c/h from wLaunchElf 8d4a0c2 by AKuHAK and SP193
libcdvd_add.c/h & OSDInit.c/h from PS2Ident v0.835 by l_Oliveira and SP193

v0.42
Experimental FMCB support mc1
Removed versions strings/release dates
Code optmizations

v0.41
Correct release date of OPL
Minor text display adjustments

v0.4
Minor code cleanup
Removed few debug messages
Added support for ESR
Bump OPL to r1650

v0.3
Can now use different paths and devices!
Can select mc0 or mass
Can select FORTUNA or APPS
No more sub folders
Source Code released

v0.2
Added GSM
Added PS2Ident
Added many more RetroArch Cores
Now Initializes DVD Drive and stops CD if it is present.

v0.1
First release
pad.c and pad related functions from wLaunchElf.elf 8d4a0c2
Function ResetIOP() from main.c MPLUS-LOADER3.ELF
Function LoadElf() from main.c MPLUS-LOADER3.ELF </pre>
