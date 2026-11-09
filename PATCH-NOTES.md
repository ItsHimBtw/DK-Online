# DK Online — Helkar compatibility patch

Core source: verified full upstream 4.2.0 Dashboard-and-Client. Compatibility release: v4.2.0-helkar.1.

- Fixed all seven readers for 565/567-byte item records, including the inserted raw tag and 16-bit equipment-set ID. Dungeon/event/quest references, shops, boxes and GM lookup now use the shared layout.
- Kept the new tag as raw data; no gameplay meaning was guessed. Both layouts and set IDs above 255 have regression coverage. All 96,060 supplied compiled item records decode without uncovered nonzero bytes, and full fresh preparation completes.
- Isolated Evocatoon (Summoner skill 3196, ten levels) because its supplied source lacks aggro definition 1167. Learning, books, reinforcement and casting are blocked before costs; other validation remains active. The dashboard and tooltip explain the limitation.
- Fixed dashboard startup confirmation to check the server app, installation, prepared-data/code versions and process ID instead of matching a displayed product name.
- Applied the new transparent gold emblem to project PNG/ICO/SVG assets and all 20 product executables, plus setup; icons include seven sizes. Renamed the experimental native components; see COMPONENTS.md.
- Removed shared test-account seeding and personal/development state from the release package. Bundled official Node and preserved upstream runtime/library notices.
- Added standalone Windows setup, bundled runtime handling and verified safe extraction. Basic file-backed setup needs no Git, compiler, manual Node or SQL installation. Microsoft WebView2 is installed from its signature-checked official bootstrap when absent.

## Verified and limited

Generated compatibility tests, fresh preparation, bundled-runtime planning with a system-only PATH, native configuration resolution and a ten-frame native renderer check passed. ZIP/installer files were checked against a SHA-256 manifest. The dashboard started a local-file world; client visual gameplay was not exercised.

Broader Helkar effects and dungeon symptoms still need a specific in-client reproduction. Existing source-data holes are reported rather than invented. Native gameplay/protocol parity, remote hosting and a factory-clean Windows 10/11 machine are not certified. The setup wrapper is unsigned. Automatic in-app updates are disabled for this compatibility build; use the release downloads.

## Content and attribution

Original game packs, executable, GameGuard, extracted game caches, fonts/music, accounts and personal configuration are excluded. Supply your own compatible local game installation and do not redistribute its prepared cache. The normal dashboard world uses the Node engine; the separate native suite remains experimental.

Upstream: https://github.com/MagicIbrar/DK-Engine/releases/tag/v4.2.0 . Contributors and third-party notices are preserved. No project-wide open-source license, clean-room provenance or legal clearance is claimed; no rights to original game materials are granted.
