# MacBook Lid Frosted Glass Effect

FrostFold v0.8 is an experimental macOS menu-bar app that creates a progressive frosted-glass overlay with perspective compensation as a supported MacBook lid closes.

## Download

[Download FrostFold v0.8 for Apple Silicon](FrostFold-v0.8-macOS-arm64.zip?raw=true)

Requires macOS 15 or later, Apple Silicon, and a compatible lid-angle sensor. This is an experimental ad-hoc-signed build, not Apple-notarized. Do not weaken macOS security protections to open it.

## Use

1. Unzip and open FrostFold.app. Quit an older copy first.
2. Grant Input Monitoring for the lid sensor and Screen Recording for the temporary desktop snapshot when requested; relaunch if needed.
3. Enable the effect from the menu bar. The reference angle is 115 degrees.
4. Optional: enable camera assistance, sit normally with the lid at 113–117 degrees, then select the 115-degree calibration action and enter approximate eye-to-screen distance.
5. Turn camera assistance off, or quit FrostFold, to stop camera processing.

## Privacy

Desktop snapshots and camera frames are processed only in local memory; they are not saved or uploaded. Camera assistance is off by default and estimates viewing position only. The app does not use microphone audio, analytics, or networking.

This repository contains only the privacy-cleaned install ZIP and this guide. It excludes personal photos, desktop screenshots, local settings, caches, source paths, and build intermediates.

## Limitations

Camera distance is approximate and needs initial calibration. With multiple faces, side views, or tracking loss, the app smoothly falls back to hinge-only compensation. The camera moves with the lid and may lose the viewer at low lid angles. The overlay uses a frozen desktop snapshot rather than a live desktop.

Build and bundle checks passed, but real-device tracking accuracy, hardware compatibility, and animation quality still require physical testing.
