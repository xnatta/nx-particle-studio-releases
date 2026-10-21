# NX Particle Studio

Windows x64 particle authoring editor for FiveM. Download the installer from [Releases](https://github.com/xnatta/nx-particle-studio-releases/releases).

This is a **release-only repository**. Application source and editable reference assets are maintained separately.

The first release is an authoring alpha: native-scale reference mannequin, live 3D particles, layers, timing, lifetime curves, custom textures, project save/recovery, Thai/English UI, and experimental CodeWalker XML / DDS / YPT export.

Binary export requires a separately installed trusted CodeWalker folder. YPT files have been structurally reloaded with CodeWalker; in-game rendering in FiveM has not been validated. Mesh/trail/flipbook authoring and multiplayer synchronization are not yet included.

Updates are checked in the installed app. Downloading and installation require explicit actions. Work is saved to recovery before exit; projects/settings are outside the replaceable program directory. SHA-512 validation and a staged helper protect the install process. Installers are currently unsigned.

Versioned release assets are immutable. Each installer has a SHA-256 sidecar; `latest.yml` is used by the app updater. No publisher credentials are shipped.
