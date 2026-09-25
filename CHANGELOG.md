# Changelog

## Unreleased

- Fix Blur my Shell's application blur showing nothing (translucent but unblurred windows): apply the rounded corners effect to the window's content (surface container), never the whole window actor, and move it there if it was attached before the surface appeared.
- Stop logging criticals when a window closes after Blur my Shell removed its blur.
- Fix border and blur keeping a window's initial size when it resizes right after opening (they only caught up on the next manual resize).
- Fit the Blur my Shell blur from the window's frame/buffer rects (always current) instead of actor allocations, and refit it on every window resize.
- Blur my Shell compatibility: fit its application blur (static and dynamic) to the rounded, padded window shape, so no square blurred corners or edges show around translucent windows.

## v2.2.0

- Add GNOME 50 compatibility fixes for the rounded-corners shader path.
- Round Wayland-native, X11/XWayland, Qt, Electron, Firefox, VS Code, Thunderbird, and LibreOffice top-level windows more reliably.
- Match windows using WM_CLASS, Wayland app IDs, and desktop IDs.
- Avoid duplicate effect and shadow attachment during complex window startup.
- Clarify installation and Wayland limitations in the documentation.