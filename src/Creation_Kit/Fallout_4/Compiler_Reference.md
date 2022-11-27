# Fallout 4 Papyrus Compiler Reference

## CLI Reference

```text
Papyrus Compiler Version 2.8.0.4 for Fallout 4
Copyright (C) ZeniMax Media. All rights reserved.
Usage:
PapyrusCompiler <object, folder, or project> [<arguments>]

  object     Specifies the object to compile. (-all is not specified, with a
             .psc or no extension)
  folder     Specifies the folder to compile. (-all is specified)
  project    Specifies the project to compile. (Has a .ppj extension)
  arguments  One or more of the following (overrides project, if any):
   -debug|d
    Turns on compiler debugging, outputting dev information to the screen.
   -release|r
    Turns on release-mode processing, removing debug code from the script.
   -final
    Turns on final-mode processing, removing beta code from the script.
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
   -norecurse
    Used with -all to tell the compiler not to recurse into subdirectories.
   -ignorecwd
    Tells the compiler to ignore the current working directory when searching
    for files. Otherwise it is implied to be first in the import list.
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
