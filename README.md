# SingStar Toolbox
A Custom Disc Creator for SingStar. 

Combine **existing SingStar discs**, create **custom discs** with your own songs, **now with PS3 + FTP support!**

Also includes tools for various formats used by SingStar games (**PAK, PKD, PKF, IPU, MIB, IAV, CHC** etc..)

**Tutorials/Guide:** [Check out the Wiki](https://github.com/RavenDS/singstar-toolbox/wiki)

**Join the Discord server for help:** [https://discord.gg/jNet59FPVz](https://discord.gg/jNet59FPVz)

<img src="Singstar-Toolbox-1.1.png" width=50% height=50%>

### Main Features
- Import & convert UltraStar songs (txt)
- Import songs from official SingStar discs to use in your own (PS2/PS3)
- Convert audio & video to proprietary SingStar format (IPU + MIB)
- Build an ISO compatible with emulators & real hardware (PS2/PS3)

### QoL Features
- No external tools (apart from ffmpeg)
- M2V to IPU converter (no SDK needed)
- Audio normalization for consistent volume
- Entirely rewritten TXT to XML converter
- Support for regular, duet, rap songs
- Fix text encoding automatically
- & much more..

### Setup & Requirements
- [Getting started (recommended)](https://github.com/RavenDS/singstar-toolbox/wiki/Getting-Started-(Setup-&-Requirements))
- #### Download the latest version of ffmpeg.exe <a href="https://www.gyan.dev/ffmpeg/builds/ffmpeg-git-full.7z">(direct link for Win10)</a> and place it in the same folder as Singstar Toolbox.
- .NET 8.0 Desktop Runtime

# Roadmap 
### In progress
- [ ] **GLOBAL:** Drag & Drop songs (TXT & SSTP)
- [ ] **PS4:** Import songs from SingStar PS4
- [ ] **PS2:** Build NTSC PS2 discs
- [x] **GLOBAL:** Import/Convert SING-IT to SingStar

### Completed ([v1.4](https://github.com/RavenDS/singstar-toolbox/releases/latest))
- [x] **GLOBAL:** Extract audio from video (for .TXTs with video only)
- [x] **GLOBAL:** Convert PS2 songs to PS3
- [x] **GLOBAL:** Convert PS3 multi-channel audio to stereo for PS2 (no loss)
- [x] **GLOBAL:** Convert PS3 songs to PS2
- [x] **GLOBAL:** Edit videos to include time gap
- [x] **GLOBAL:** Scale BPM & notes when BPM is too high
- [x] **ISO:** ISO Rebuilding
- [X] **PS3:** PS3 Full Support
- [x] **PS3:** Export/Build PS3 Data
- [x] **PS3:** Auto-decrypt supported ISOs when needed
- [x] **PS3:** Update existing song library via FTP
- [x] **PS3:** NTSC video support
- [x] **PS2:** PAK file Unpacking/Repacking
- [x] **PS2:** M2V to IPU conversion
- [x] **PS2:** Import songs from NTSC discs (IAV+IND)
- [x] **PS2:** IPU swizzling
- [x] **PS2:** 99% codec compatibility
- [x] **PS2:** Audio Encode to ADPCM
- [x] **PS2:** MIB + MIH export 
- [x] **PS2:** BMP to TX2 + TX2 to BMP
- [x] **PS2:** Import songs from other discs
- [x] **PS2:** Edit/disable menu music
- [x] **PS2:** Multiple Language support (English, French, German, Italian)

### Scrapped/Cancelled
- **yt-dlp support:** Many UltraStar managers already handle this
- **Edit PS2 boot logos:** Users can edit that from DiscData folder
- **Medley Editor:** Would require a lot of user input. Not cancelled but very low priority. Medleys are currently automated.

# Source code
Source code is available as multiple modules and tools that will be published gradually.
- [IPUenc](https://github.com/RavenDS/IPUenc) (IPU<->M2V video)

# Credits
- Chris [(@christphen)](https://github.com/christphen) joined the project as a collaborator
- <a href="https://ffmpeg.org/">ffmpeg</a>
- [DiscUtils.Iso9660](https://github.com/DiscUtils/DiscUtils)
- [NAudio](https://github.com/naudio/NAudio)
- [Ude.NetStandard](https://github.com/errepi/ude)
- [nQuant](https://www.nuget.org/packages/nQuant)
- [ss_cover.cc](https://github.com/performous/performous-tools/blob/master/ss_cover.cc) *(TX2 to BMP conversion)*
- [scee-london](https://github.com/EdnessP/scee-london) *(PKD unpacking)*
- [BouncyCastle](https://www.bouncycastle.org/download/bouncy-castle-c/) *(Whirlpool Hash)*
- Holger Kuhn (hawkear@gmx.de) for his work on SingStar overall
- Special thanks to [@locastan](https://github.com/locastan) for his help

## Notes
It is possible to add more than 100 songs to a single PS2 disc, however it might cause unexpected behaviour in-game.
<br />**PS3 isn't affected by this.**
