# scripts-manager

Helps updating/maintaining scripts in *PATH*

## Intro

With the irruption of git, maintaing scripts becomes easier and easier. That ends with a pletora of repos providing some kind of functionality. If you use a bunch of them, but want to keep in touch with new changes, best way is to clone repo, and symlink script to *PATH*.

    $ git clone <url_repo> <repo>
    $ cd <repo>
    $ ln -s $PWD/<script> ~/bin #suppose ~/bin is in *PATH*

## Features

Locate symlinks in *PATH* and test if they are under git control. Then ask to fetch updates if there were any.

## Improvements

- Config on search dirs in *PATH*
- Allow to push changes (if repos are yours, that's another task you want to automate)

