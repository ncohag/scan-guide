# Scan Guide

iPhone web app that walks through a photogrammetry scan plan (from asset-forge's `scan_planner`) shot by shot:
where to stand, phone height, live turn/tilt meters, auto-shoot when lined up, zip export.

Open https://ncohag.github.io/scan-guide/ in Safari, then Share → Add to Home Screen.
Desktop test: add `?sim` to the URL for heading/tilt sliders.

## Markers

Print `markers/scan_markers_letter.pdf` (100% / Actual size) or 3D-print the two-colour tiles in `markers/`.
With markers the app tracks the phone's real position (distance, height, angle) from AprilTag 36h11 tags,
calibrates the lens and the compass itself, and guides you in centimetres. The PC pipeline (`markers.py`)
reads the same tags for true scale and the object's front/up.
