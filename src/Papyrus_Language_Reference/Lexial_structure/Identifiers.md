# Identifiers

> **<sup>Lexer:</sup>**\
> LETTER : [`a`-`z`] | [`A`-`Z`]
>
> DIGIT : [`0`-`9`]
>
> IDENTIFIER: (LETTER | `_`) (LETTER | DIGIT | `_`)<sup>\*</sup> <sub>Except [Keywords](./Keywords.md)</sub>

> **<sup>Lexer Fallout 4:</sup>**\
> NAMESPACED_IDENTIFIER: IDENTIFIER (`:` IDENTIFIER)<sup>\*</sup>

Identifiers start with either an ASCII letter or an underscore and are followed by any amount of letters, digits or underscores. An identifier can contain only letters and only underscores.

The following identifiers are valid:

- `a`
- `_`
- `_a`
- `_0`
- `a_`
- `_0_`
- `_______`

The following identifiers are invalid:

- `0`
- `ä`
- `あ`
- `a-b`

## Namespaces

Fallout 4 added Namespaces to the language which can be used to better reference other [Scripts](../Concepts/Scripts.md). A namespaced identifier uses multiple identifiers separated by columns (`:`):

```papyrus
ScriptName Quests:MyQuest:Script1
```

Namespaced identifiers can be used whenever referencing a script:

```papyrus
ScriptName Quests:MyQuest extends Quest

; Quests:OtherQuest is another Script that extends "Quest"
Quests:OtherQuest Property TheOtherQuest Auto Const
```
