<div align="center">

# FlowVid

**Stream movies and shows across desktop, mobile, and TV.**

[**flow-vid.com**](https://flow-vid.com) &nbsp;·&nbsp; [**Download**](https://flow-vid.com/downloads)

</div>

---

FlowVid is a commercial, closed-source app. This organization hosts the **open-source components** it is built on and has modified, each published under its original license.

### Media playback (mpv + FFmpeg)

FlowVid plays video with [mpv](https://github.com/mpv-player/mpv) and [FFmpeg](https://ffmpeg.org), built under the **LGPL** (no GPL or nonfree components) so they can be used in a closed-source app while fully honoring those licenses.

- [**flowvid-libmpv-desktop**](https://github.com/flow-vid/flowvid-libmpv-desktop): LGPL libmpv for the desktop app (Windows `.dll` + Linux `.so`), plus the Tauri mpv plugin (MPL-2.0).
- [**flowvid-mpv-winbuild-cmake**](https://github.com/flow-vid/flowvid-mpv-winbuild-cmake): the pinned Windows build recipe for the above.
- [**android-mpv**](https://github.com/flow-vid/android-mpv): LGPL libmpv for the mobile and TV apps.
- [**flowvid-media3-ffmpeg**](https://github.com/flow-vid/flowvid-media3-ffmpeg): LGPL FFmpeg audio decoder for AC-3, E-AC-3, DTS, MLP and TrueHD, packaged as an AAR for Media3.
- [**flowvid-libdovi-android**](https://github.com/flow-vid/flowvid-libdovi-android): MIT libdovi JNI bridge for Profile 7 MEL to Profile 8.1 metadata conversion on Android.

Each component is built and published in compliance with the licenses of its upstream project.

Security issues in these components should be reported privately through the repository's
**Security** tab. Product support and general feedback belong at
[flow-vid.com/support](https://flow-vid.com/support), not in build-recipe issue trackers.

---

<div align="center">
Get the FlowVid apps at <a href="https://flow-vid.com/downloads"><b>flow-vid.com/downloads</b></a>
</div>
