# DVDemu demo discs and DVDemu Share

Free DVD-Video disc images for trying [DVDemu](https://acolytelabs.com), built from open films,
and **DVDemu Share**, which streams your own disc images to DVDemu from a computer on your home network.
Each disc has real DVD menus, chapters, audio tracks and subtitles.

## Download

See [Releases](../../releases) for the ISO files.

| Disc | Size | Contents |
|---|---|---|
| Tears of Steel (2012) | 521 MB | 12-minute film, 5.1 + stereo audio, 9 subtitle languages, scene selection, extras |

## How to use

- **Phone or tablet:** download the ISO, open DVDemu, tap **+**, choose "A folder on this device", and pick the folder holding the ISO (for example, Downloads).
- **Android TV:** copy the ISO to a USB drive, plug it into the TV, then press **+** and choose that drive.

## DVDemu Share

Keep your ISO files on a PC or Raspberry Pi and play them on any phone, tablet or TV running DVDemu.
Download it from [Releases](../../releases).

**Windows:** run `DVDemu-Share.exe` (Windows on ARM: `DVDemu-Share-ARM.exe`). It asks for the folder
holding your ISO files, then sits in the system tray. When Windows Firewall asks, allow it on private
networks. Windows may warn that the app is from an unknown publisher: choose **More info > Run anyway**.

**Raspberry Pi or Linux:** pick the file for your system (`vdv-share-linux-arm64` for a Pi 3/4/5 on
64-bit Raspberry Pi OS, `-armv7` for 32-bit, `-armv6` for a Pi Zero or Pi 1, `-x64` for a PC or NAS), then:

```sh
chmod +x vdv-share-linux-arm64
sudo ./vdv-share-linux-arm64 install-service -folder /path/to/your/ISOs
vdv-share code      # the pairing code, if a device asks for one
```

**Pairing:** with Share running, open DVDemu on the same network. The computer shows up by itself
(or tap **+ > A computer by its address**). Tap **Pair** and allow it on the computer, or type the
6-digit code it shows. Its discs then appear on your shelf.

## Credits

Tears of Steel (c) 2012 Blender Foundation | mango.blender.org.
Licensed under [Creative Commons Attribution 3.0](https://creativecommons.org/licenses/by/3.0/).
Subtitles by the Mango project and its volunteer translators.
The disc authoring (menus and layout) is by Acolyte Labs.
