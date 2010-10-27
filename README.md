# git-empty-dirs

Makes git look like it handles empty directories.


## Installation

Add "bin" to your "$PATH" before git's location (which bin/git expects to be
"/usr/bin", but you can change that easily).


## Usage

git-status will now remind you of directories which are untracked because
they're empty. Track them by doing "git add <dir>/.gitkeep", like my git-status
says.

You can then commit your addition and the file will hide forever. And I don't
mean "hidden" because its name begins with a dot, it really won't be there
to clutter your filesystem. You can delete it (and the folder it protects) by
using "git-rm <dir>".


## Bugs

The ".gitkeep" files will show up in git-archive's tarballs.
Use the provided "tar-stripkeep" to get rid of them.
