# Skyrim Papyrus Compiler Reference

## CLI Reference

```text
Usage:
PapyrusCompiler <object or folder> [<arguments>]

  object     Specifies the object to compile. (-all is not specified)
  folder     Specifies the folder to compile. (-all is specified)
  arguments  One or more of the following:
   -debug|d
    Turns on compiler debugging, outputting dev information to the screen.
   -optimize|op
    Turns on optimization of scripts.
   -output|o=<string>
    Sets the compiler's output directory.
   -import|i=<string>
    Sets the compiler's import directories, separated by semicolons.
   -flags|f=<string>
    Sets the file to use for user-defined flags.
   -all|a
    Invokes the compiler against all psc files in the specified directory
    (interprets object as the folder).
   -quiet|q
    Does not report progress or success (only failures).
   -noasm
    Does not generate an assembly file and does not run the assembler.
   -keepasm
    Keeps the assembly file after running the assembler.
   -asmonly
    Generates an assembly file but does not run the assembler.
   -?
    Prints usage information.
```

