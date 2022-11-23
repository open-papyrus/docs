# Scripts

> **<sup>Syntax:</sup>**\
> _ScriptHeader_ :\
> &nbsp;&nbsp;`ScriptName` [IDENTIFIER] (`extends` [IDENTIFIER])<sup>?</sup> _ScriptFlags_<sup>\*</sup> [EOL]
>
> _ScriptFlags_ : [IDENTIFIER]

> **<sup>Syntax Fallout 4:</sup>**\
> _ScriptHeader_ :\
> &nbsp;&nbsp;`ScriptName` [NAMESPACED_IDENTIFIER] (`extends` [NAMESPACED_IDENTIFIER])<sup>?</sup> _ScriptFlags_<sup>\*</sup> [EOL]
>
> _ScriptFlags_ :\
> &nbsp;&nbsp;`BetaOnly` |\
> &nbsp;&nbsp;`Const` |\
> &nbsp;&nbsp;`DebugOnly` |\
> &nbsp;&nbsp;`Native` |\
> &nbsp;&nbsp;[IDENTIFIER]

## Source File

Papyrus source files have the extension `.psc` and can use any of the valid [Encodings] and [Line Endings]. The file name **must be** the same as the identifier in the Script Header. The Script Header **must be** the first line in the file that is neither a comment nor an empty line.

```papyrus
; MyScript.psc
ScriptName MyScript
```

Fallout 4 added [Namespaced Identifiers](../Lexial_structure/Identifiers.md#namespaces) which are identifiers separated by columns (`:`). Each Identifier of a Namespaced Identifier must be the parent of the next Identifier in the File System.

```papyrus
; Quests/MyQuest/Script1.psc
ScriptName Quests:MyQuest:Script1
```

## Script Flags

The only valid flags that can be applied to a Script in **Skyrim** are [User-defined Flags].

**Fallout 4** added the following keywords as flags.

- `BetaOnly`
- `Const`
- `DebugOnly`
- `Native`

## Documentation

The Script Header can be followed by a [Documentation Comment] that describes the Script.

[IDENTIFIER]: ../Lexial_structure/Identifiers.md
[NAMESPACED_IDENTIFIER]: ../Lexial_structure/Identifiers.md#namespaces
[EOL]: ../Lexial_structure/Whitespace.md#line-endings
[Encodings]: ../Lexial_structure/Whitespace.md#encoding
[Line Endings]: ../Lexial_structure/Whitespace.md#line-endings
[User-defined Flags]: ../Lexial_structure/Flags.md#user-defined-flags
[Documentation Comment]: ../Lexial_structure/Comments.md#documentation-comments
