---
title: "Writing Your First Payload"
description: "Making CatScratch payloads on the USB Nugget"
lead: "Making CatScratch payloads on the USB Nugget"
date: 2020-10-13T15:21:01+02:00
lastmod: 2020-10-13T15:21:01+02:00
draft: false
images: []
menu:
  docs:
    parent: "guides"
weight: 120
toc: true
---
<img src="/images/payload.gif" title="Payload Image"/>
<br /><br />

The USB Nugget supports CatScratch, making it easy to create your first payload!

If you need inspiration, you can find a list of payloads on the Hak5 GitHub repository](https://github.com/hak5/usbrubberducky-payloads), which can be converted to CatScratch with our [converter tool](https://github.com/RetiaLLC/Nugget_Tools).

To get started, let’s review the full list of CatScratch commands the USB Nugget supports.

### CatScratch Payload Structure

When writing a CatScratch payload, commands are executed line by line. It's also possible to press multiple keys at the same time by putting commands on the same line!

To write out a piece of text, type TYPE in all caps.  See the example below for how this works:
| Example        | Result                                             |
|----------------|----------------------------------------------------|
| SHIFT C        | Type the Shift key and then the c key              |
| SHIFT C        | Press the Shift key and the c key at the same time |
| TYPE Hello     | Types out "Hello"                                  |

### Built-in Commands
Now that we have the basics down, let's take a look at supported commands:
| Command                             | Example               | Description                                                                                                                  |
|-------------------------------------|-----------------------|------------------------------------------------------------------------------------------------------------------------------|
| `//`                                | `// Some comment`     | This is used to leave comments, and is not executed in the script                                                            |
| `DEFAULTWAIT`  or  `DEFAULT_WAIT`   | `DEFAULTWAIT 200`     | This sets the default time in ms between each command                                                                        |
| `WAIT`                              | `WAIT 1000`           | Sets a one-time delay in ms                                                                                                  |
| `TYPE`                              | `TYPE Hello World!`   | Types whatever string follows the command                                                                                    |
| `LED`                               | `LED R`               | Changes the color of the LED. Current Options:  R = red, G = green, B = blue, C = cyan, Y = yellow, M = magenta,  W = white  |
| `SCREEN`                            | `SCREEN Hello`        | Displays the string after the command on the USB Nugget's screen                                                             |

### Supported Keys
Most standard keys are supported by the Rubber Nugget.
| Key                   |
|-----------------------|
| `a`-`z`               |
| `A`-`Z`               |
| `1`-`9`               |
| `F1`-`F12`            |
| `!@#$%^&*()_-=+`, etc |

### Modifier Keys
Keys like SHIFT, ALT, and the WINDOWS or GUI key can be useful for accessing hotkey combinations, are are frequently used in combination key presses.
| Key                      |
|--------------------------|
| `CTRL`  or  `CONTROL`    |
| `SHIFT`                  |
| `ALT`                    |
| `WINDOWS` `CMD` or `GUI` |

### Other Useful Keys
Virtually anything you can do behind a keyboard can be recreated with the right keypresses. 
The following keys are essential to trigger keyboard shortcuts and navigate without a mouse.
| Key               |
|-------------------|
| `ENTER`           |
| `MENU`  or  `APP` |
| `DELETE`          |
| `HOME`            |
| `INSERT`          |
| `PAGEUP`          |
| `PAGEDOWN`        |
| `UP` or `UPARROW` |
| `DOWN` or `DOWNARROW`
| `LEFT` or `LEFTARROW`
| `RIGHT` or `RIGHTARROW`
| `TAB`
| `END`
| `ESC` or `ESCAPE`
| `SPACE`
| `PAUSE` or `BREAK`
| `CAPSLOCK`
| `NUMLOCK`
| `PRINTSCREEN`
| `SCROLLLOCK`

Now that we've gone over the supported CatScratch commands, let's load and deploy a payload to the USB Nugget.
