# ConsoleWriter
A basic console writer that allows for quick coloring and formatting of console print

## Write() Function
### Usage
This function is used to print formatted text to the console
### Parameters
- **text** _(string)_: The text you want to print into the console
- **autoReturn** _(bool)_ _Default: false_: Signals whether to make a new line or not
- **foreground** _(string)_ _Default: gray_: The text/foreground color of the line (see "Console Colors" below)
- **background** _(string)_ _Default: black_: The background color of the line
```
ConsoleWriter.Write("Some Text",true,"green","white");
```

## Rewrite() Function
### Usage
This function is used to overwrite the text on the currently selected line
_NOTE_: it defaults to cursor position 0 on the current line
### Parameters
- **text** _(string)_: The text you want to print into the console
- **autoReturn** _(bool)_ _Default: false_: Signals whether to make a new line or not
- **foreground** _(string)_ _Default: gray_: The text/foreground color of the line (see ConsoleColors below)
- **background** _(string)_ _Default: black_: The background color of the line
```
ConsoleWriter.Rewrite("Some Text",true,"green","white");
```

## Blank() Function
### Usage
This function is used to print a blank line to the console
#### Parameters
**_NONE_**
```
ConsoleWriter.Blank();
```

## Console Colors
### Description
This a list of colors that you can use for the foreground and background parameters

#### Allowed colors
- black
- blue
- cyan
- darkblue
- darkcyan
- darkgray
- darkgreen
- darkmagenta
- darkred
- darkyellow
- gray
- green
- magenta
- red
- white
- yellow

# Upcoming Changes
- Make the Rewrite() command have additional optional parameters for specifying the cursor position
- Make the Rewrite() clear the line before posting OR make it aware of the prior character count on the line and apply an appropriate ammount of spaces to compensate
- Adjust both Rewrite() and Write() to adjust the incoming foreground and background colors to lowercase
