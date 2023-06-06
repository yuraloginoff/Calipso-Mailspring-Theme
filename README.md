# Maria Mailspring Theme

Theme for the [Mailspring](http://www.getmailspring.com/) email client. Inspired by Darkside theme that comes out of the box and [Nord](https://www.nordtheme.com/) color palette.

<img src="https://raw.githubusercontent.com/yuraloginoff/Maria-Mailspring-Theme/master/screenshot/screenshot.jpg" />

## Motivation

I want Trash button to be floated on left side of top bar. It always should be at the same position. Now it's not fixed, as you probably know.

I want
<img src="https://raw.githubusercontent.com/yuraloginoff/Maria-Mailspring-Theme/master/screenshot/good.png" />
instead of
<img src="https://raw.githubusercontent.com/yuraloginoff/Maria-Mailspring-Theme/master/screenshot/bad.png" />


My solution:
```CSS
.sheet-toolbar .message-toolbar-items {
  order: -300;
}

.sheet-toolbar .message-toolbar-items .button-group:first-child {
  flex-direction: row-reverse;
}
```

## How to install
1. Clone this repo or Download the code.
2. Decompress the zip file.
3. Open `Mailspring` -> `Install new theme...` and select folder.