# Keywords

Keywords are **case-insensitive** meaning you can write them in complete UPPERCASE, lowercase or anything in between. All keywords are _reserved_ and cannot be used as [identifiers](./Identifiers.md).

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
> KW_PARENT: `Parent`\
> KW_PROPERTY: `Property`\
> KW_RETURN: `Return`\
> KW_SCRIPTNAME: `ScriptName`\
> KW_SELF: `Self`\
> KW_STATE: `State`\
> KW_STRING: `String`\
> KW_TRUE: `True`\
> KW_WHILE: `While`

The following keywords were added in Fallout 4.

> **<sup>Lexer Fallout 4:</sup>**\
> KW_BETAONLY: `BetaOnly`\
> KW_CONST: `Const`\
> KW_CUSTOMEVENT: `CustomEvent`\
> KW_CUSTOMEVENTNAME: `CustomEventName`\
> KW_DEBUGONLY: `DebugOnly`\
> KW_ENDGROUP: `EndGroup`\
> KW_ENDSTRUCT: `EndStruct`\
> KW_GROUP: `Group`\
> KW_IS: `Is`\
> KW_SCRIPTEVENTNAME: `ScriptEventName`\
> KW_STRUCT: `Struct`\
> KW_STRUCTVARNAME: `StructVarName`\
> KW_VAR: `Var`

<div class="warning">

The `Parent` and `Self` keywords are special variables and treated as identifiers by both the Skyrim and Fallout 4 Creation Kit compilers, meaning the following code will compile. Custom compilers **should** fail to compile this code as it is not functional.

```papyrus
int Parent = 0
int Self = 0
```

</div>
