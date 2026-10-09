# Turemin firmware

Firmware images for **Turemin**, a touchless synthesizer that is played with both hands above two
distance sensors (ESP32-S3).

This repository only contains release builds. The source code is not public.

## Updating

In the Turemin app: **Firmware → Check for updates → Install**. The board needs a WiFi connection
with internet access (home network).

Every release contains:

- `turemin.bin` – the application image
- `version.json` – version, size and SHA-256 of the image

The board only switches to a new image if its size and SHA-256 match, and it returns to the
previous firmware by itself if the new one does not start properly.
