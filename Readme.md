# DK Online 4.2.0 — Helkar compatibility build

![DK Online gold emblem](dk-online-gold-emblem.png)

[Download Windows setup](https://github.com/ItsHimBtw/DK-Online/releases/latest/download/DK-Online-Setup-4.2.0.exe) · [Download complete ZIP and sources](https://github.com/ItsHimBtw/DK-Online/releases/latest/download/DK-Online-Clean-Release-4.2.0.zip) · [Patch notes](PATCH-NOTES.md)


Run DK-Online-Setup-4.2.0.exe, or extract the ZIP and open DK Online.exe. Select your own compatible, updated local Global installation when asked. Setup uses the bundled Node runtime, checks/automatically installs Microsoft WebView2 if needed, prepares a separate local asset cache and opens the dashboard. Use Start world, then open the client yourself. Windows 10/11 x64 and its .NET Framework are the supported target; internet is needed if WebView2 is absent. SQL is optional for basic local play. No Git, compiler or manual Node setup is required.

This archive contains engine/tools and the new project emblem. It contains no original game packs, executable, extracted maps/models/textures, fonts, sound, original logos or GameGuard. Never redistribute an installed copy or prepared cache: those contain the player's locally supplied game data.

Known limitation: Evocatoon is quarantined because its supplied source data lacks aggro definition 1167; other supported content remains available. See VALIDATION.md. Helkar is the update name confirmed by the user. General effects/dungeon symptoms still need a concrete reproduction/source comparison; no blanket fix is claimed.

The core source comes from the verified full 4.2.0 DK Engine release: https://github.com/MagicIbrar/DK-Engine/releases/tag/v4.2.0 . Its attribution and upstream library/runtime notices are retained. The experimental native components are separately renamed project components; the basic dashboard world uses the supplied Node engine. This package does not establish code ownership, clean-room provenance, original-client parity or legal clearance. No rights to the original game's materials are granted, and this project is independent of its owners. See ASSET-PROVENANCE.md and 3 - Dashboard/THIRD_PARTY_NOTICES.md.

Downloads and patch notes: https://github.com/ItsHimBtw/DK-Online/releases . Automatic in-app updates are disabled for this compatibility build; install updates from that release page. Core source version: 4.2.0; compatibility release tag: v4.2.0-helkar.1.

