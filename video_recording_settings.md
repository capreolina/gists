# My setings for recording MapleLegends

## MapleLegends

### Legends\.ini

```ini
[RESOLUTION]
; This sets your resolution for MapleLegends
; 0 = 800x600
; 1 = 1024x768
; 2 = 1366x768 (Unstable on MAC)
HDClient = 2

[MODS]
; Run client in windowed mode
; Put on false if you prefer starting in full-screen mode
; In-game you can also press ALT + ENTER to toggle between windowed and full-screen
Windowed = true

; Start the client in the center of the screen.
StartInCenter = false

; Have the client remember the position in which the client was closed last time, and open up in that position.
; StartInCenter will override this, so make sure to have StartInCenter set to false if you want this to work.
RememberClosePos = false

; This skips the starting logo animation screens and sends you straight to login.
SkipWizetAnim = true

; Enable darker chat background, which helps you seeing the chat in bright areas
DarkChat = true

; Enable infinite chat logging, which allows you to see everything said in-game from your game session without it erasing
InfiniteChatLog = true

; Select the type of transitioning between maps. This affects the duration and speed of the dark screen during map transfer.
; 1 = Classic MapleStory
; 2 = Modern MapleStory
; 3 = MapleLegends' Own Tweaks
Transition = 3

; Enable the Streamer Mode, which hides the login ID in the Title screen and in the Cash Shop.
StreamerMode = true
```

### In-game settings

- SYSTEM OPTIONS
    - **PICTURE QUALITY:** BEST
    - **SHAKE UP THE SCREEN:** false
    - **MONSTER INFO.:** Mark name and HP

## OBS

### Settings

- Output
    - Recording
        - **Recording Format:** mp4
        - **Rescale Output:** false
        - \[encoder settings\]
            - **Codec:** H\.264
            - **Profile:** High
            - **Level:** 5\.2
            - **Rate Control:** CQP
            - **QP:** 18
            - **Keyframe Interval:** auto
    - Audio
        - Track `n`
            - **Audio Bitrate:** 320
- Audio
    - General
        - **Sample Rate:** 44\.1 kHz
        - **Channels:** Stereo
- Video
    - **Base (Canvas) Resolution:** 1280x720
    - **Output (Scaled) Resolution:** 1280x720
    - **Downscale Filter:** Bilinear
    - **FPS:** 60
- Advanced
    - Video
        - **Color Format:** NV12
        - **Color Space:** 709
        - **Color Range:** Partial

### Canvas layout

Just a “Window Capture” of the MapleLegends window. With this selected, you can right click ▶ “Transform” ▶ “Edit Transform…” to get to the “Edit Transform” window. The settings here are:

- **Position:** (0, 0)
- **Rotation:** 0
- **Size:** (1280, 720)
- **Positional Alignment:** Top Left
- **Bounding Box Type:** No bounds
- Crop
    - **Left:** 0
    - **Right:** 0
    - **Top:** 0
    - **Bottom:** 0
        
Also by right clicking the preview with the MapleLegends window element selected, you can do “Scale Filtering” ▶ “Disable” to disable filtering when downscaling to the 1280×768 canvas.
