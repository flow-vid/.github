<div align="center">

# FlowVid

**Your library, on every screen. Movies and shows across desktop, phone and TV.**

[**flow-vid.com**](https://flow-vid.com) &nbsp;·&nbsp; [**Download**](https://flow-vid.com/downloads) &nbsp;·&nbsp; [**Support**](https://flow-vid.com/support)

</div>

---

FlowVid is free to use. An optional **Supporter** subscription adds extras such as hosting watch
parties and themes; everything else, including playback, your library, profiles and sync, is free
for everyone.

The FlowVid apps themselves are not open source. This organization hosts the **open-source
components** they are built on, exactly as FlowVid builds and ships them, so anyone can see what
runs inside the apps and rebuild those parts. Nothing here is relicensed: every repository keeps
its upstream license and its full history.

### How FlowVid plays video

- **Desktop (Windows, Linux):** [mpv](https://github.com/mpv-player/mpv), embedded through a small
  Tauri plugin.
- **Android and Android TV:** the platform's own player, [ExoPlayer (Media3)](https://github.com/androidx/media),
  for the widest hardware support including Dolby Vision and HDR, with mpv as a second engine for
  formats and subtitles the platform player handles less well. FlowVid picks between them
  automatically and you can override it.

mpv and [FFmpeg](https://ffmpeg.org) are built here under the **LGPL** with no GPL or nonfree
components, which is what allows them to be used inside a closed-source app while fully honoring
those licenses. ExoPlayer is Apache-2.0 and is used as published by Google; FlowVid's small
modifications to it live inside the apps and are credited there.

### The repositories

- [**flowvid-libmpv-desktop**](https://github.com/flow-vid/flowvid-libmpv-desktop): LGPL libmpv for
  the desktop app (Windows `.dll` and Linux `.so`), plus the Tauri mpv plugin (MPL-2.0).
- [**flowvid-libmpv-windows-recipe**](https://github.com/flow-vid/flowvid-libmpv-windows-recipe):
  the pinned Windows build recipe used by the repository above. Scripts only, no binaries.
- [**flowvid-libmpv-android**](https://github.com/flow-vid/flowvid-libmpv-android): LGPL libmpv for
  the phone and TV apps.
- [**flowvid-ffmpeg-android**](https://github.com/flow-vid/flowvid-ffmpeg-android): LGPL FFmpeg
  audio decoder for AC-3, E-AC-3, DTS, MLP and TrueHD, packaged as an AAR for Media3.
- [**flowvid-libdovi-android**](https://github.com/flow-vid/flowvid-libdovi-android): MIT libdovi
  JNI bridge that converts Dolby Vision Profile 7 metadata to Profile 8.1 on Android.

Each component is built and published in compliance with its upstream project's license, from
pinned sources, with checksums and build provenance attached to every release. The Windows build
recipe carries no license of its own because its upstream publishes none.

### Getting in touch

- **Using FlowVid?** Help and feedback live at [flow-vid.com/support](https://flow-vid.com/support).
- **Found a security issue in one of these components?** Report it privately through that
  repository's **Security** tab.
- **Something wrong with a build here?** Open an issue on that repository.

---

<div align="center">
Get the FlowVid apps at <a href="https://flow-vid.com/downloads"><b>flow-vid.com/downloads</b></a>
</div>
