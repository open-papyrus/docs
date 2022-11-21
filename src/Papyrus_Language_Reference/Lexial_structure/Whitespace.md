# Whitespace

> **<sup>Lexer:</sup>**\
> WHITESPACE : `U+0009` | `U+000D` | `U+0020`
>
> LINE_ENDING : `U+000A`
>
> LINE_TERMINATOR : `\`
>
> EOL : WHITESPACE<sup>\*</sup> LINE_TERMINATOR<sup>?</sup> WHITESPACE<sup>\*</sup> LINE_ENDING

The following is a list of valid whitespace characters.

- `U+0009`: horizontal tab
- `U+000D`: carriage return
- `U+0020`: space

Whitespace characters only serve to separate _tokens_ in the grammar, and have no semantic significance. This is different to programming languages such as Python or markup languages like YAML where indentation matters.

## Line Endings

Both `LF` and `CRLF` are valid line endings because the Creation Kit compilers separate lines on `U+000A` (line feed) and `U+000D` (carriage return) is treated as whitespace.

## Encoding

Files **should** be encoded using `UTF-8` however because of the limited character set allowed by the Creation Kit compilers, other encodings that share the following code points are also allowed (`UTF-16-LE`, `UTF-16-BE`, `UTF-32`):

- [`0`-`9`] must start at `0x30` (`0`) and end at `0x39` (`9`)
- [`A`-`Z`] must start at `0x41` (`A`) and end at `0x5A` (`Z`)
- [`a`-`z`] must start at `0x61` (`a`) and end at `0x7A` (`z`)

## Line Terminators

In order for [Statements] to be separated correctly, languages must define a separator. Conventional languages like C++, C# or Java use a semi-column (`;`) to separate statements, but Papyrus uses line endings instead. This means only one statement is allowed per line. Papyrus allows statements to be split on multiple lines using the backslash character (`\`).

```papyrus
int x = 0 +\
1
```

The backslash **must** be followed by any amount of whitespace and a [Line Ending](#line-endings). The following is not valid Papyrus code.

```papyrus
int x = 0+\ ; comment after line terminator is not allowed
1
```
