# Validation scope

The actual source release is the full 4.2.0 Dashboard-and-Client package (SHA-256 3a6b30a4b07997a97961ec88e22f0764ccd54eebf2babbf53968ffc25edce15a). It was compared with the earlier mixed package; this build uses that verified 4.2.0 dashboard/client plus the renamed experimental native suite.

The newer 567-byte compiled item layout inserts a tag at offset 137 and widens the equipment-set index to 16 bits. Fields after those positions shift; this build corrects all seven item consumers, including dungeon/event/quest ticket/name lookup, shops, rewards and GM indexes. Both 565/567 layouts have generated regression fixtures. The tag is retained without inventing gameplay semantics. A synthetic set ID 256 reaches runtime set-bonus calculation. All 96,060 real compiled item records decode with no uncovered nonzero bytes; full preparation completed from the selected original packs.

Evocatoon (Summoner staff Grand Meister skill 3196, ten levels) references missing aggro definition 1167 in those packs. Only that confirmed unsupported skill is blocked from learning, books, reinforcement and casting; its records and raw references stay intact. Its tooltip and dashboard health explain the limitation. Other invalid references still fail validation. No invented aggro data is supplied.

The bundled Node runtime and installation planning passed with a system-only PATH. The package checks/bootstraps Microsoft WebView2 when missing, uses Windows .NET Framework, and defaults basic local play to files rather than requiring SQL. No Git, compiler or manual Node install is needed for basic setup. A disposable clean Windows machine was not available; this is not a factory-clean Windows certification.

The vague reported missing effects/dungeon gameplay symptoms have not been visually reproduced. Shared item decoding fixes are proven; complete effects, every dungeon, renderer/protocol parity and remote hosting are not certified. Automatic in-app updates are disabled for this compatibility build; use the verified release downloads.
