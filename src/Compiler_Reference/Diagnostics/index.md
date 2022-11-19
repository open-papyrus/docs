# Diagnostics

The following pages list all diagnostics created during a compilation step. In general each diagnostic has the following attributes:

- **Prefix**: 1-character literal, unique to the compilation step
- **ID**: 3-digit number, unique to the diagnostic in the compilation step
- **Level**: one of the [Severity Levels](#severity-levels)
- **Message**: explanation of the diagnostic

## Severity Levels

### Error

An error thrown during compilation will halt the entire process and requires a fix.

### Warning

A warning does not halt compilation however it shows potential issues in the code such as performance issues and unnecessary work.

### Suggestion

A suggestion does not halt compilation and provide tips to improve your code which don't fall in other severity levels.
