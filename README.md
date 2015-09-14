## tmsu-tagd
ncurses ui dialog script for editing [TMSU](https://github.com/oniony/TMSU) tags of one file

#### Usage
`$ tmsu-tagd ./file` will open ncurses ui checklist with available tags.

To add new tags and values use:
```
$ tmsu-tagd ./file new_tag newtag2=value
```

Hit `<Escape>` or press `Cancel` to abort changes. Press `OK` to apply chosen tags.
Hit letter keys to place cursor at tag with matching first letter.

You may want to create easier symbolic link `ln -s ./tmsu-tagd tagd`

#### Dependencies
  - [TMSU](https://github.com/oniony/TMSU)
  - dialog
  - ncurses

#### Known Issues
  - only arguments within `[A-Za-z_0-9]` character set are handled correctly, for best experience do not use special characters or whitespace
  - currently no way to use database other than `~/.tmsu/default.db`
