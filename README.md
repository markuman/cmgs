mygithub
====

mygithub helps you to clone and keep sync all you own repositories and all your stared repositories.

- Verion 6
 * improve third option input. it's set to "justme" now.

- Version 5
 * support mirroring only repositories from given username
 * e.g. $ ./mygithub markuman /mnt/GITHUB/ justme
 * it's a weak implementation, because it doesn't matter what kind of string the third option is!

- Version 4
 * remove cat dependency
 * fix bug while extracting own repositories

- Version 3
 * rename cmgs to mygithub
 * clone/pull stars and own github repositories
 * mkdir -p for destination dir

- Version 2
 * implement pull if repository already exist

- Version 1
 * initial release


# REQUIREMENTS
 wget, grep, cut, git, sed

# USAGE

    # Make it executable
    $ chmod u+x mygithub
    
    # Clone all repositories from user USERNAME incl his/her stared repositories
    $ ./mygithub USERNAME destinationFolder
    
    # Clone just the repositories from user USERNAME
    $ ./mygithub markuman /srv/http/viewgit/my-github-mirror/ justme
