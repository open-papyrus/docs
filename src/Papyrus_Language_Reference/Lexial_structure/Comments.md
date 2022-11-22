# Comments

> **<sup>Lexer:</sup>**\
> SINGLE_LINE_COMMENT : `;` ~[EOL]<sup>\*</sup> [EOL]
>
> MULTI_LINE_COMMENT : `;/` ~`/;`<sup>\*</sup> `/;`
>
> DOCUMENTATION_COMMENT : `{` ~`}`<sup>\*</sup> `}`

There are three types of comments:

* [Single-line Comments](#single-line-comments)
* [Multi-line Comments](#multi-line-comments)
* [Documentation Comments](#documentation-comments)

## Single-line Comments

These comments start with a `;` and end at the [Line Ending]. Anything within the comments will be ignored by the compiler.

```papyrus
; this is a comment
int x = 0 ; this is also a comment
int y = 0; this is also valid
```

## Multi-line Comments

Multi-line comments start with a `;/` and end at a `/;`. These comments swallow line endings.

```papyurs
;/
this
can
go
across
multiple
lines
/;

int x = 0;/ it can even
start here
/;
```

## Documentation Comments

These comments **can only** appear after one of the following concepts and will be visible in the editor.

- [Script Header](../Concepts/Scripts.md)
- [Property Definitions](../Concepts/Properties.md)
- [Function Definitions](../Concepts/Functions.md)
- [Event Definitions](../Concepts/Events.md)

Fallout 4 added Documentation Comments to more concepts:

- [Property Group Definition](../Concepts/Properties.md)
- [Struct Member Definition](../Concepts/Structures.md)

Between a concept and a Documentation Comment can be any amount of whitespace and empty lines. Because Single-line and Multi-line Comments are ignored the following code is valid.

```papyrus
ScriptName MyScript

; Single-line comments are skipped

;/
so are Multi-line Comments
/;

{Documentation Comments can appear
after any amount of empty lines.}
```

[WHITESPACE]: ./Whitespace.md
[EOL]: ./Whitespace.md
[Line Ending]: ./Whitespace.md#line-endings
