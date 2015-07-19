# scripts-manager

Helps updating/maintaining scripts in *PATH*

## Intro

With the irruption of git, maintaining scripts becomes easier and easier. That ends with a pletora of repos providing some kind of functionality. If you use a bunch of them, you want to keep in touch with new changes. 

You can see a lot of influence from this script in vim script manager like [Vundle](https://github.com/gmarik/Vundle.vim). That's intentional.

## Install 

Clone repo, and symlink script to *PATH*.

    $ git clone <url_repo> <repo>
    $ cd <repo>
    $ ln -s $PWD/<script> ~/bin #suppose ~/bin is in *PATH*

## Use

Show `--help` for examples. basically

    script-manager -u do what you want

An useful function you can define on your startup scripts

    function cd-script {
       cd $(script-manager --goto=$@)
    }
    
    $ cd-script <empty-or-filter>

## Features

Locate symlinks in *PATH* and test if they are under git control. Then ask to fetch updates if there were any.

## Improvements

- Config on search dirs in *PATH*
- Allow to add, commit, merge and push changes (if repos are yours, that's another task you want to automate)
- Rudimentary edit projects
- metadata managed scripts

## Get involved

find *TODOs* on script to locate the exact task you can help with.

