# ConsoleWriter
A basic console writer that allows for quick coloring and formatting of console print

## Usage
### Write() Function
#### Parameters
- **text** _(string)_: The text you want to print into the console
- **autoReturn** _(bool)_: Signals whether to make a new line or not
- **foreground** _(string)_: The text/foreground color of the line (see ConsoleColors below)
- **background** _(string)_: The background color of the line
```
ConsoleWriter.Write("Some Text",true,"green","white");
```

### Rewrite() Function
#### Usage
This function is used to overwrite the text on the currently selected line
_NOTE_: it defaults to cursor position 0 on the current line
##### Parameters
- **text** _(string)_: The text you want to print into the console
- **autoReturn** _(bool)_: Signals whether to make a new line or not
- **foreground** _(string)_: The text/foreground color of the line (see ConsoleColors below)
- **background** _(string)_: The background color of the line
```
ConsoleWriter.Rewrite("Some Text",true,"green","white");
```

### Blank() Function
#### Usage
This function is used to print a blank line to the console
##### Parameters
**_NONE_**
```
ConsoleWriter.Blank();
```
