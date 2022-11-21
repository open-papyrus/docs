# Flags

Flags are modifiers that can be applied [Scripts](../Concepts/Scripts.md), [Properties](../Concepts/Properties.md), [Variables](../Concepts/Variables.md) and [Functions](../Concepts/Functions.md). There are two types of flags:

- [Flags as Keywords](#keywords)
- [User-defined Flags](#user-defined-flags)

## Keywords

These flags are [Keywords](./Keywords.md) meaning they are _reserved_ and can not be used as identifiers.

> **<sup>Lexer:</sup>**\
> KW_AUTO: `Auto`\
> KW_AUTOREADONLY: `AutoReadOnly`\
> KW_NATIVE: `Native`

The following flags were added in Fallout 4.

> **<sup>Lexer Fallout 4:</sup>**\
> KW_BETAONLY: `BetaOnly`\
> KW_CONST: `Const`\
> KW_DEBUGONLY: `DebugOnly`

## "User-defined Flags"

The Creation Kit compilers accept a `.flg` file containing "User-defined Flags". The flags defined in these files are not part of the Creation Kit compilers because they are not relevant to the game, only the editor. These flags **should not** be treated as [Keywords](./Keywords.md) since they can be used as [Identifiers](./Identifiers.md).

### Skyrim (`TESV_Papyrus_Flags.flg`)

```txt
// List of flags for TESV - DO NOT EDIT

// Flag hides the script or property from the game editor
Flag Hidden 0
{
	Script
	Property
}

// Flag on an object designates it as the script the condition system will look at
// Flag on a variable allows the script variable to be examined by the condition system
Flag Conditional 1
{
	Script
	Variable
}
```

### Fallout 4 (`Institute_Papyrus_Flags.flg`)

```txt
// List of flags for Institute - DO NOT EDIT

// Flag hides the script or property from the game editor
Flag Hidden 0
{
	Script
	Property
	StructVar
}

// Flag on an object designates it as the script the condition system will look at
// Flag on a variable allows the script variable to be examined by the condition system
Flag Conditional 1
{
	Script
	Variable
}

// Flags the specified script as a default script, for filtering in the editor
Flag Default 2
{
	Script
}

// Flags this group as collapsed on the reference in the editor
Flag CollapsedOnRef 3
{
	Group
}

// Flags this group as collapsed on the base object in the editor
Flag CollapsedOnBase 4
{
	Group
}

// Flags this group as collapsed (on both ref and base) in the editor
Flag Collapsed CollapsedOnRef & CollapsedOnBase

// Flags a property as mandatory - in other words, will spit out a warning in
// the editor if it isn't given a value
Flag Mandatory 5
{
	Property
}
```
