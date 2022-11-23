# Terminology

This section covers the various terms used throughout the documentation.

- **Lexer**: converts the raw code into a list of [Tokens](https://en.wikipedia.org/wiki/Lexical_analysis#Token)
- **Parser**: takes the output of the lexer and creates an [Abstract Syntax Tree](https://en.wikipedia.org/wiki/Abstract_syntax_tree) (AST)
- **Lowering**: "lowers" the AST into an [Intermediate Representation](https://en.wikipedia.org/wiki/Intermediate_representation#Intermediate_representation) (IR)
- **Intermediate Representation**: different representation of the code than the AST, better suited for analysis and optimization
- **Backend**/**Code Generator**: converts the IR into the final output (the `.pex` file)
