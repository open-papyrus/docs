# Keywords

Keywords are divided into these categories:

- [Reserved keywords](#reserved-keywords)
- [Special identifiers](#keyword-is-identifier)

Keywords are **case-insensitive** meaning you can write them in complete UPPERCASE, lowercase or anything in between.

## Reserved keywords

These keywords are _reserved_ and cannot be used as [identifiers](./Identifiers.md).

> **<sup>Lexer:</sup>**\
> KW_AS: `As`\
> KW_AUTO: `Auto`\
> KW_AUTOREADONLY: `AutoReadOnly`\
> KW_BOOL: `Bool`\
> KW_ELSE: `Else`\
> KW_ELSEIF: `ElseIf`\
> KW_ENDEVENT: `EndEvent`\
> KW_ENDFUNCTION: `EndFunction`\
> KW_ENDIF: `EndIf`\
> KW_ENDPROPERTY: `EndProperty`\
> KW_ENDSTATE: `EndState`\
> KW_ENDWHILE: `EndWhile`\
> KW_EVENT: `Event`\
> KW_EXTENDS: `Extends`\
> KW_FALSE: `False`\
> KW_FLOAT: `Float`\
> KW_FUNCTION: `Function`\
> KW_GLOBAL: `Global`\
> KW_IF: `If`\
> KW_IMPORT: `Import`\
> KW_INT: `Int`\
> KW_LENGTH: `Length`\
> KW_NATIVE: `Native`\
> KW_NEW: `New`\
> KW_NONE: `None`\
> KW_PROPERTY: `Property`\
> KW_RETURN: `Return`\
> KW_SCRIPTNAME: `ScriptName`\
> KW_STATE: `State`\
> KW_STRING: `String`\
> KW_TRUE: `True`\
> KW_WHILE: `While`

## Keyword is identifier

These keywords **are** [Identifiers](./Identifiers.md) and carry special meaning.

> **<sup>Lexer:</sup>**\
> KW_PARENT: `Parent`\
> KW_SELF: `Self`

<div class="warning">

`Parent` and `Self` are treated as identifiers by the Creation Kit Compiler meaning the following is valid Papyrus code but should not be used:

```papyrus
int Parent = 0
int Self = 0
```

</div>
