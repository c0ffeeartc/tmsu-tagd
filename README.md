## tmsu-tagd
ncurses dialog shell script for editing [TMSU](https://github.com/oniony/TMSU) tags of one file

#### Usage
`$ tmsu-tagd ./file` will open ncurses ui checklist with available tags.

To add new tags and values use:
`$ tmsu-tagd ./file new_tag newtag2=value` will add new tags to list and enable them.

Hit `<Escape>` or press `Cancel` to abort changes. Press `OK` to untag --all, and then retag with chosen tags.
Hit letter keys to place cursor at tag with matching first letter.

You may want to create easier symbolic link `ln -s ./tmsu-tagd tagd`

#### Dependencies
  - [TMSU](https://github.com/oniony/TMSU)
  - dialog
  - ncurses

