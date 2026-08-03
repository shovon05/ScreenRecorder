# 📱 Lightweight Screen Recorder (Optimized Fork)

A highly optimized, privacy-focused, and lightweight screen recording application for Android. 

This repository is a customized fork of the original ScreenRecorder project, heavily modified to prioritize performance, reduce CPU/memory overhead, and eliminate background bloat.

## ✨ Key Enhancements & Features

*   **Zero GC Churn:** Audio encoding loops have been rewritten to prevent Garbage Collection spikes, ensuring buttery-smooth performance.
*   **Optimized Video Output:** Hardcoded to 25 FPS at 4 Mbps (H.264/AAC) for crystal-clear, professional 1080p video without massive file sizes.
*   **Maximized Audio Capture:** Bypasses strict audio limitations by capturing `USAGE_UNKNOWN` channels, allowing for the broadest possible system audio recording (Note: Android OS restricts direct VoIP capture; use speakerphone for meetings).
*   **Invisible Overlay:** Floating controls use `FLAG_SECURE` removal and smart auto-collapsing to stay out of your final video.
*   **R8 Minification:** Debug bloat has been stripped out, resulting in a tiny, highly efficient `.apk`.

## 🚀 How to Download & Install

You don't need Android Studio to compile this app! It builds automatically using GitHub Actions.

1. Go to the [Actions tab](../../actions) in this repository.
2. Click on the latest successful **Build Android App** workflow.
3. Scroll down to the **Artifacts** section.
4. Download the `app-release-unsigned-apk.zip` file.
5. Extract the zip and install the `.apk` directly to your Android device.

## 🛠️ Build it Yourself

If you wish to fork this project and build it via GitHub Actions:
1. Fork this repository.
2. Navigate to the **Actions** tab in your new fork and enable workflows.
3. Go to the `.github/workflows/build.yml` file and trigger a run.
4. Download your newly compiled APK from the artifacts!

---
*Maintained and optimized by [Shovon](https://github.com/shovon05)*
