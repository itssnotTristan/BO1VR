# BO1VR

An experimental Windows PCVR extension for **Call of Duty: Black Ops**.
This repository hosts downloads, setup information and bug reports. The full
development repository and native C++ source are maintained privately.

[**Download BO1VR**](../../releases) Â· [Report a bug](../../issues/new/choose)

## Requirements

- Your own installed Steam PC copy of Call of Duty: Black Ops. Start the
  original single-player game once, then close it before installing BO1VR.
- Windows and a working PCVR headset connection with an OpenXR runtime.
- Scope: solo Campaign, solo Zombies and private Steam Zombies co-op.

Game content comes from the player's installation. The download contains no
original game executable, maps, extracted models, textures or audio.

## Install or update

1. Download the release asset ending in **-portable.zip**. GitHub's automatic
   Source code ZIP/tar.gz contains this website's docs, not an installable mod.
2. Close Black Ops. Extract the portable ZIP beside **BlackOps.exe** in the
   original Steam game folder. Merge the Bo1VR folder when updating.
3. Preserve `players`, `bo1vr.ini` and `Bo1VR/.local`; they hold your personal
   settings, saves and poses. Run **Bo1VR.bat** from the game folder.

The package also contains controls, release notes, verification limits and
download troubleshooting. Use **Bo1VR-Check.bat** if installation/launch fails.

## Current test build

**0.1.0-test23-coop109** fixes the extended MAC-10 magazine detachment,
automatic CZ75 reload-part selection and chamber continuity on partial magazine
swaps. It softens hover highlighting, seats the knife contact toward the wrist,
restores native TOW steering input and adds trigger-only underbarrel launcher
mechanisms. See the bundled CONTROLS-coop109.txt and verification report.

The original BO1 cloth pouch still prepares from the player's own retail files.
The optional pose-import executable reported in coop107 remains excluded; saved
poses and holster editing remain available. No antivirus setting is changed.

This is a test build. Physical-headset feel, two-PC private co-op and complete
Campaign stability are not certified. Include your exact build, map/mission,
headset and OpenXR runtime in reports. See [SUPPORT.md](SUPPORT.md).

## Source and notices

The core C++ source is private. The current download contains readable launcher
scripts and C# helpers needed by the existing tools. Project MIT terms and
dependency notices are retained; private hosting does not replace those terms.
See [LICENSE](LICENSE), [CREDITS.md](CREDITS.md) and the bundled notices.

Call of Duty: Black Ops belongs to its respective owners. This is an unofficial
extension. Implementation and testing are AI-assisted with OpenAI Codex.
