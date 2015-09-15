## tmsu-tagd
ncurses ui dialog script for editing [TMSU](https://github.com/oniony/TMSU) tags of one file

#### Usage

To edit file's tags:
```
$ tmsu-tagd ./file
```

To edit tags and add new tags and values:
```
$ tmsu-tagd ./file new_tag newtag2=value
```

You may want an easier to type shell command `ln -s ./tmsu-tagd tagd`

Dialog checklist provides following hotkeys:

  - `<Up>`, `<Down>` - select next/previous tag
  - `<Left>`, `<Right>` - select button to press on `<Enter>`
  - Letter keys - position cursor onto next tag with matching first key
  - `<Space>` - toggle current checklist element
  - `OK` button - apply changes and exit
  - `Cancel` button, `<Esc>` - cancel changes and exit

#### Dependencies
  - [TMSU](https://github.com/oniony/TMSU)
  - dialog
  - ncurses

#### Known Issues
  - only arguments within `[A-Za-z_0-9]` character set are handled correctly, for best experience do not use special characters or whitespace
  - currently no way to use database other than `~/.tmsu/default.db`
