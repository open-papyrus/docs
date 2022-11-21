# Identifiers

> **<sup>Lexer:</sup>**\
> LETTER : [`a`-`z`] | [`A`-`Z`]
>
> DIGIT : [`0`-`9`]
>
> IDENTIFIER: (LETTER | `_`) (LETTER | DIGIT | `_`)<sup>\*</sup> <sub>Except [Keywords](./Keywords.md)</sub>

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
