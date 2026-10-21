# NX Particle Studio

Windows x64 particle authoring editor for FiveM. Download the installer from [Releases](https://github.com/xnatta/nx-particle-studio-releases/releases).

This is a **release-only repository**. Application source and editable reference assets are maintained separately.

Version 0.3.0 adds custom particle image import directly in the lower-left library. Choose a static PNG, WebP or JPG/JPEG, inspect its checkerboard preview and Import and apply. Transparent white PNG at 512 or 1024 square is recommended. Black → alpha is optional for light textures on black. Proportions are preserved with transparent square padding, capped at 2048 px without upscaling. Images and filename metadata stay embedded in each project and recovery; export converts them to DDS automatically. Limits: 12 MB per source image, 32 million source pixels, 16384 px per source side, 64 imported images and 64 MB per project. Animated images/SVG/DDS/YPT/model files are not image-import inputs.

Version 0.2.0 adds ten independent movement choices: rise, outward, inward, orbit, helix, vortex, wave, figure-eight, custom spline and static. Every choice supports continuous or burst emission and Once/Loop playback. Use New → Spring lights to start a helix around the native-scale mannequin; adjust its turns, dimensions, travel, spin and direction, or convert it to editable points. The editor also includes layers, lifetime curves, custom textures, save/recovery and Thai/English UI.

Motion export uses generated client.lua together with static native point effects in the YPT. Keep the whole resource together; path trajectories are driven by Lua. Export has a conservative 256 simultaneous-handle budget. Binary export requires a separately installed trusted CodeWalker folder. YPT files have been structurally reloaded with CodeWalker; in-game rendering/follow behavior in FiveM has not been validated. Mesh/trail/flipbook authoring and multiplayer synchronization are not yet included.

Updates are checked in the installed app. Downloading and installation require explicit actions. Work is saved to recovery before exit; projects/settings are outside the replaceable program directory. SHA-512 validation and a staged helper protect the install process. Installers are currently unsigned.

Versioned release assets are immutable. Each installer has a SHA-256 sidecar; `latest.yml` is used by the app updater. No publisher credentials are shipped.
