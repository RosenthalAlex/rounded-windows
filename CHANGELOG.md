# Changelog

## Unreleased

- Blur my Shell compatibility: fit its application blur (static and dynamic) to the rounded, padded window shape, so no square blurred corners or edges show around translucent windows.

## v2.2.0

- Add GNOME 50 compatibility fixes for the rounded-corners shader path.
- Round Wayland-native, X11/XWayland, Qt, Electron, Firefox, VS Code, Thunderbird, and LibreOffice top-level windows more reliably.
- Match windows using WM_CLASS, Wayland app IDs, and desktop IDs.
- Avoid duplicate effect and shadow attachment during complex window startup.
- Clarify installation and Wayland limitations in the documentation.