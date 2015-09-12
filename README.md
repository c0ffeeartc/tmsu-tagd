## tmsu-tagd
ncurses dialog shell script for editing [TMSU](https://github.com/oniony/TMSU) tags of one file

#### Usage
`$ tmsu-tagd ./file` will open ncurses ui checklist with available tags.

Hit `<Escape>` or press `Cancel` to abort changes. Press `OK` to untag --all, and then retag with chosen tags.

#### Dependencies
  - [TMSU](https://github.com/oniony/TMSU)
  - dialog
  - ncurses

#### Known Issues
  - Adding new tags/values isn't yet supported
