# Scripts

> **<sup>Syntax:</sup>**\
> _ScriptHeader_ :\
> &nbsp;&nbsp;`ScriptName` [IDENTIFIER] (`extends` [IDENTIFIER])<sup>?</sup> _ScriptFlags_<sup>\*</sup> [EOL]

> **<sup>Syntax Fallout 4:</sup>**\
> _ScriptHeader_ :\
> &nbsp;&nbsp;`ScriptName` [NAMESPACED_IDENTIFIER] (`extends` [NAMESPACED_IDENTIFIER])<sup>?</sup> _ScriptFlags_<sup>\*</sup> [EOL]

## Source File

Papyrus source files have the extension `.psc` and can use any of the valid [Encodings] and [Line Endings]. The file name **must be** the same as the identifier in the Script Header.

```papyrus
; MyScript.psc
ScriptName MyScript
```

Fallout 4 added [Namespaced Identifiers](../Lexial_structure/Identifiers.md#namespaces) which are identifiers separated by columns (`:`). Each Identifier of a Namespaced Identifier must be the parent of the next Identifier in the File System.

```papyrus
; Quests/MyQuest/Script1.psc
ScriptName Quests:MyQuest:Script1
```

[IDENTIFIER]: ../Lexial_structure/Identifiers.md
[NAMESPACED_IDENTIFIER]: ../Lexial_structure/Identifiers.md#namespaces
[EOL]: ../Lexial_structure/Whitespace.md#line-endings
[Encodings]: ../Lexial_structure/Whitespace.md#encoding
[Line Endings]: ../Lexial_structure/Whitespace.md#line-endings
