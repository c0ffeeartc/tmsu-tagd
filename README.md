## tmsu-tagd
ncurses dialog shell script for editing tmsu tags of one file

#### Usage
Running `tmsu-tagd ./file` from shell will open ncurses ui checklist with available tags.

Hit `<Escape>` or press `Cancel` to abort changes. Hit `OK` to untag --all, and then retag with chosen tags.

#### Dependencies
  - tmsu
  - dialog
  - ncurses

#### Known Issues
  - Adding new values isn't yet supported
  - On pressing `OK` script runs two commands, `tmsu untag --all ./file` and then `tmsu tag --tags="*" ./file`, if second command fails file will loose all tags
