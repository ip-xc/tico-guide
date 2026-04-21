# tico-guide
<!-- Tagline -->
tico is the first custom emulation frontend for Nintendo Switch - a controller-first, native C++ interface designed for performance, simplicity, and long-term portability.

This guide tries to be as hands-on as possible and cover most questions along the way.

<!-- Table of Contents -->
<p align="center">
  <a href="#about">About</a> •
  <a href="#prerequisites">Prerequisites</a> •
  <a href="#deployment">Deployment</a> •
  <a href="#usage">Usage</a> •
  <a href="#faqs">Frequently Asked Questions</a> •
  <a href="#credits">Credits</a> •
</p>

# About
This is a small guide that helps you start a small media server on your local network, incorperating local files stored on your Synology NAS and using the Gelato plugin to fetch media with your debrid account.

For further details about tico, please visit their [Github repository](https://github.com/ticohq/tico).

| :warning: At the time of this guide I am running HOS 22.1.0 and tico 0.7.0. This guide might be subject to change. |
| --- |

# Prerequisites 

* **A compatible Nintendo Switch** --> please refer to one of the dozens of setup guides to see the supported models (V1, Lite & OLED).
* A way to **write and modify files** on your Switch (MTP, FTP..).

# Deployment
1. First, download the **latest** Release of tico from [Github here](https://github.com/ticohq/tico/releases).

<div><img width="1024" src="placeholder" alt="first"> </div>

2. Connect to your Nintendo Switch and open the SD cards root folder "/".

<div><img width="1024" src="placeholder" alt="second"></div>

3. **Extract and copy** the files from "**tico-release.zip**" inside the "**SD card**".

<div><img width="1024" src="placeholder" alt="third"></div>

4. When it's done, you can run it from **hbmenu** (Click on **Album while holding R**).

# Usage

< COMING SOON >

# FAQs

## Where do I download ROMs and BIOS?

A: You have to dump the data from your legally owned system.

## Where do I put my ROMs?

A: Your ROMs are put into **sdmc:/tico/roms/<SYSTEM>**. [See here for supported ROIM formats.](https://ticoverse.com/wiki/library-and-roms/supported-rom-formats).

## What are Cores and how do I install them?

A: Cores are "plug-in"-emulators that know how to run certain games for the corresponding system. You can install the Cores via **Emulator** inside **Settings**.

## I cannot find Dolphin and GameCube!

A: You have to enable Dolphin under **Experimental**.

## My GameCube games run slow!

A: Try letting it sit idle once to compile shaders. If the game crashes, try a second time. The build is still in alpha.

## My PSX / Dreamcast / Sega devices won't run!

A: You need the proper BIOS file for the system and put them inside **sdmc:/tico/system/<SYSTEM>**.

## I get an SSL / SSH error when downloading Covers / Cores / etc.

A: Be sure that your time settings are correctly set to the current date/time.

## My ROMs are not being found?

A: Check your ROMs folder on your SD card. The file layout is supposed to look like this:

```plain
/sdmc/                                          
├── /tico/                                     
│   ├── /roms/                         <-- ROMs folder
│   │   ├── /gba/                      <-- Console
│   │   │   ├── game1.gba              <-- ROM for corresponding console
│   │   │   └── ..
│   │   ├── /wii/
│   │   │   ├── game1.iso
│   │   │   └── ..
│   │   ├── /gc/
│   │   │   ├── game1.iso
│   │   │   └── ..
│   ├── /system/
│   │   ├── /psx/                      <-- Console folder
│   │   │   ├── bios.bin               <-- BIOS for corresponding console
│   │   └── ..
│   ├── /cores/                        <-- Cores folder
│   │   ├── /<EMULATOR-tiicu>/         <-- Emulator for corresponding console
│   │   │   └── <EMULATOR-ticuu.nro    <-- Core for corresponding console
│   │   ├── /<EMULATOR-tiicu>/
│   │   │   └── <EMULATOR-ticuu.nro
│   ├── ..
│   │   │
```

If it looks good, Rescan the games when you hover over the system and click on **Rescan Games**.

# Credits
tico for creating the frontend including custom cores - [Github repository](https://github.com/ticohq) or their [Website](https://ticoverse.com/).
