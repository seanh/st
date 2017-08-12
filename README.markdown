seanh's st
==========

This is my "fork" of [st](http://st.suckless.org/) that includes
[my custom `config.h` file](config.h) on
[this custom seanh branch](https://github.com/seanh/dwm/tree/seanh).
The `seanh` branch is branched off `master`, which tracks suckless's
`master` branch. See a
[comparison of the `seanh` branch to `master`](https://github.com/seanh/st/compare/master...seanh).

Customisations
--------------

* Ubuntu Mono font
* Dracula theme from [this patch](http://st.suckless.org/patches/dracula/)
* Tmux as the default shell

Installation
------------

```bash
sudo apt install git libxft-dev
git clone 'https://github.com/seanh/st.git' ~/.st
cd ~/.st
sudo make clean install
```

Then run `st`, and see `man st`.

If you want to add Gnome desktop integration you can add a
`~/.local/share/applications/st.desktop` file like this:

    [Desktop Entry]
    Name=st
    GenericName=Terminal
    Comment=A simple terminal implementation for X.
    Exec=st -c st
    Terminal=false
    Type=Application
    Encoding=UTF-8
    Icon=terminal
    Categories=System;TerminalEmulator;
    Keywords=shell;prompt;command;commandline;cmd;

Keyboard Shortcuts
------------------

These aren't changed from st's defaults:

<kbd>Ctrl-Shift-c</kbd> Copy the selected text to the clipboard.

<kbd>Ctrl-Shift-v</kbd> Paste from the clipboard.

<kbd>Ctrl-Shift-y</kbd> or middle mouse button: paste from primary selection.

<kbd>Ctrl-Shift-Page Up</kbd> increase font size.

<kbd>Ctrl-Shift-Page Down</kbd> decrease font size.

<kbd>Ctrl-Shift-Home</kbd> default font size.
