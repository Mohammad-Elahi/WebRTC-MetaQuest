# [WebRTC-MetaQuest](https://github.com/Mohammad-Elahi/WebRTC-MetaQuest)

Pre-compiled WebRTC implementation optimized for Android-based AR/VR headsets using arm64-v8a architecture.

## Overview

This repository provides ready-to-use WebRTC libraries specifically built for Android-based AR/VR headsets like Meta Quest, Pico, HTC Vive Focus, and other devices running on arm64-v8a architecture. Building WebRTC from source for these devices can be extremely challenging - I've done the hard work for you!

## Compatibility

This WebRTC implementation is optimized for:

- **Target OS**: Android (including custom Android variants like Horizon OS, Pico OS)
- **Target CPU**: arm64-v8a architecture
- **Build type**: Release (optimized, non-debug)
- **Supported devices**:
    - Meta Quest 2, Quest 3, Quest Pro
    - Pico 4, Pico Neo series
    - HTC Vive Focus series
    - Magic Leap 2
    - Xreal/Nreal devices
    - Lenovo ThinkReality
    - Other Android-based XR headsets


## Features

- **Low-latency communication** essential for immersive XR experiences
- **Optimized performance** for ARM64 processors (Snapdragon XR chipsets)
- **C++ NDK compatibility** for native Android development
- **Simplified integration** into existing XR projects
- **Support for audio and video streaming** with minimal latency
- **Data channel functionality** for sending arbitrary data
- Suitable for XR collaboration, remote rendering, streaming, and more


## Technical Details

- **Target OS:** Android (including custom Android variants for XR)
- **Target CPU:** arm64-v8a (64-bit ARM)
- **Build type:** Release (optimized, non-debug)
- **Build command used:**

```
gn gen out/AndroidRelease --args='target_os="android" target_cpu="arm64" is_debug=false'
ninja -C out/AndroidRelease
```

- **Intended for:** Standalone AR/VR headsets and Android devices with ARM64 processors


## Integration

Simply download the WebRTC libraries from this repository and include them in your Android NDK C++ project.
You can link the libraries via your `CMakeLists.txt` or `Android.mk` as needed—no additional build steps required.

## XR SDK Compatibility

You can use this library with the [Meta OpenXR SDK](https://github.com/meta-quest/Meta-OpenXR-SDK) or other OpenXR-based frameworks to develop advanced XR applications for Meta Quest and similar devices.

- [Meta OpenXR SDK Download](https://developers.meta.com/horizon/downloads/package/oculus-openxr-mobile-sdk/)
- [WebRTC Native Android Documentation](https://webrtc.github.io/webrtc-org/native-code/android/)


## Author

Mohammad Elahi, TU Dresden, Vodafone Chair, mohammad.elahi@mailbox.tu-dresden.de

## How to Cite

If you use this library in your research or product, please cite it as follows:

Elahi, M. (2025). WebRTC-MetaQuest: Pre-compiled WebRTC library for Android-based AR/VR headsets (arm64-v8a). GitHub. https://github.com/Mohammad-Elahi/WebRTC-MetaQuest

For BibTeX:

```
@software{Elahi2025,
  author = {Elahi, Mohammad},
  title = {WebRTC-MetaQuest: Pre-compiled WebRTC library for Android-based AR/VR headsets (arm64-v8a)},
  year = {2025},
  publisher = {GitHub},
  journal = {GitHub repository},
  url = {https://github.com/Mohammad-Elahi/WebRTC-MetaQuest}
}
```


---

> **If you are looking for a reliable, native WebRTC solution for AR/VR headsets or any Android arm64-v8a device, this repository provides everything you need to get started quickly and efficiently.**

<div style="text-align: center">⁂</div>

[^1]: README.md

