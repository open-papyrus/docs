# Additional Resources

This is not the first and last project related to Papyrus. This page contains a list of other related projects that you might find useful.

## Papyrus Knowledge Bases

There is a decent amount of information available regarding Papyrus however that information is scattered throughout various sites and quality can vary greatly between them. I split these sites based on "what came first" and who copied what from where.

### Sources

- [Creation Kit Papyrus Reference (Skyrim)](https://www.creationkit.com/index.php?title=Category:Papyrus): The original Papyrus Wiki for Skyrim. Created by Bethesda and ZeniMax employees in 2011, this is the basis for almost all other knowledge bases.

- [Creation Kit Papyrus Reference (Fallout 4)](https://www.creationkit.com/fallout4/index.php?title=Category:Papyrus): This Wiki is essentially a clone of the Skyrim Wiki but with updated information regarding Fallout 4.

- [Papyrus Compiler Reference (Skyrim)](https://www.creationkit.com/index.php?title=Papyrus_Compiler_Reference): Creation Kit Papyrus compiler reference for Skyrim.

- [Papyrus Compiler Reference (Fallout 4)](https://www.creationkit.com/fallout4/index.php?title=Papyrus_Compiler_Reference#Optimize): Creation Kit Papyrus compiler reference for Fallout 4.

- [Differences from Skyrim to Fallout 4](https://www.creationkit.com/fallout4/index.php?title=Differences_from_Skyrim_to_Fallout_4)

- [UESP (Skyrim Compiled Script File Format)](https://en.uesp.net/wiki/Skyrim_Mod:Compiled_Script_File_Format): Page from the UESP about the `.pex` file format.

- [cadpnq/papyrith (Instruction Reference)](https://github.com/cadpnq/papyrith/wiki/Instruction-Reference): GitHub Wiki page of the [Papyrith Compiler](https://github.com/cadpnq/papyrith) that contains an incomplete list of all instructions available in the compiled file format.

### Derivatives

- [joelday/papyrus-lang (Wiki)](https://github.com/joelday/papyrus-lang/wiki/Papyrus): GitHub Wiki of the [Papyrus Language Tools](https://marketplace.visualstudio.com/items?itemName=joelday.papyrus-lang-vscode) VS Code extension. This copied a lot of information from the CK Reference Wikis.

- [UESP Creation Kit Papyrus Reference Clone (Skyrim)](https://ck.uesp.net/wiki/Category:Papyrus): This is a copy of the Skyrim specific Wiki but has been updated on some pages.

- [UESP Creation Kit Papyrus References Clone (Fallout 4)](https://falloutck.uesp.net/wiki/Category:Papyrus): This is a copy of the Fallout 4 specific Wiki but has been updated on some pages.

## Tools

The [Open Papyrus Compiler](https://github.com/open-papyrus/papyrus-compiler) is not the first unofficial compiler. Aside from the official compiler that ships with the Creation Kit, here are other community developed compilers and tools:

- [Orvid/Caprica](https://github.com/Orvid/Caprica): Papyrus compiler for Fallout 4, written in C++. This project started because the author didn't want to wait for the Fallout 4 Creation Kit. It can successfully compile all vanilla Fallout 4 scripts but is not identical to the Creation Kit compiler. This compiler also has language additions like `For`, `ForEach`, `Switch` and `Do-LoopWhile`.

- [Orvid/Champollion](https://github.com/Orvid/Champollion): Papyrus decompiler and disassembler for Fallout 4, written in C++. This tool can decompile `.pex` to `.psc` files and disassemble `.pex` to `.pas`.

- [eckserah/Champollion](https://github.com/eckserah/Champollion): Fork of [Orvid/Champollion](https://github.com/Orvid/Champollion) with untested support for Fallout 76.

- [cadpnq/papyrith](https://github.com/cadpnq/papyrith): Papyrus compiler for Fallout 4, written in Common Lisp. This compiler focuses on optimizing and has a great [Comparison page](https://github.com/cadpnq/papyrith/wiki/Comparison) showcasing its features.

- [cadpnq/papyrithjs](https://github.com/cadpnq/papyrithjs): Disassembler and optimizer for Fallout 4, written in JavaScript. This tool can disassemble `.pex` to `.pas` files as well as optimize them.

- [ShikyoKira/Project-New-Reign---Open-Papyrus](https://github.com/ShikyoKira/Project-New-Reign---Open-Papyrus): Papyrus Compiler for Skyrim, written in C++. This project comes from the author of the animation tool [Nemesis](https://github.com/ShikyoKira/Project-New-Reign---Nemesis-Main). There is no meaningful information available on this project.

- [Mutagen.Bethesda.Core.Pex](https://github.com/Mutagen-Modding/Mutagen/tree/dev/Mutagen.Bethesda.Core/Pex): `.pex` parser, written in C#. Part of the [Mutagen](https://github.com/Mutagen-Modding) collection of libraries related to Bethesda modding.

- [fireundubh/pyro](https://github.com/fireundubh/pyro): Build automation for Bethesda mods (requires external compiler).

## Other

- [fireundubh/OpenPapyrus](https://github.com/fireundubh/OpenPapyrus): [ANTLR4](https://www.antlr.org/) grammars for Fallout 4 Papyrus.

- [Pickysaurus/highlightjs-papyrus](https://github.com/Pickysaurus/highlightjs-papyrus): Papyrus grammars for [highlight.js](https://github.com/highlightjs/highlight.js)

- [joelday/papyrus-lang](https://github.com/joelday/papyrus-lang): Papyrus Language Tools for VS Code, written in C#. Contains a full Language Service and Server.

- [joelday/papyrus-debug-server](https://github.com/joelday/papyrus-debug-server): Debug Adapter Protocol for Skyrim and Fallout 4. Uses a SKSE/F4SE and WebSocket to communicate with the Client.

- [nikitalita/papyrus-debug-server ](https://github.com/nikitalita/papyrus-debug-server/tree/master) fork of [joelday/papyrus-debug-server](https://github.com/joelday/papyrus-debug-server) with various modernization updates.

- [blu3mania/npp-papyrus](https://github.com/blu3mania/npp-papyrus): Notepad++ Plugin for Papyrus.

- [Kiyozz/papyrus-compiler-app](https://github.com/Kiyozz/papyrus-compiler-app): Wrapper around the CK compiler for MO2.

## Discord Servers

- [Papyrus Language Tools](https://discord.gg/E4dWujQ): Server for [joelday/papyrus-lang](https://github.com/joelday/papyrus-lang)
- [Advanced Settlement Power (redux)](https://discord.gg/X6Udqfx): Server for [cadpnq/papyrith](https://github.com/cadpnq/papyrith)
- [SkyrimSE RE](https://discord.gg/apkA9B4fnW): Server for various SKSE/F4SE plugins, mainly focused on reverse engineering.
- [Mutagen](https://discord.gg/A3jbaGe): Server for [Mutagen-Modding](https://github.com/Mutagen-Modding)
- [Modding Tools](https://discord.gg/8KHQqTw): Server for [zEdit](https://github.com/z-edit/zedit), [Cathedral-Assets-Optimizer](https://gitlab.com/G_ka/Cathedral_Assets_Optimizer) and other tools
- [xEdit](https://discord.gg/mQA5Wnu): Server for [xEdit](https://github.com/TES5Edit/TES5Edit)
- [NexusMods](https://discord.gg/nexusmods): Server for [NexusMods](https://nexusmods.com)
- [Wabbajack](https://discord.gg/Wabbajack): Server for [Wabbajack](https://wabbajack.org)
- [Mod Organizer 2](https://discord.gg/6GKR9jZ): Server for [Mod Organizer 2](https://github.com/ModOrganizer2/modorganizer)
