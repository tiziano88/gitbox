gitbox
======

gitbox allows managing files on your hard drive through git, even though they
do not live inside a git repository. The way it accomplishes this is by
copying each file or directory of your choice to a git repository, and then
replacing the originals with symlinks to the new location.

1.   fork and clone this repository to your hard drive (normally your home folder)

2.   if you want, make an alias to gitbox so you do not have to remember its
     absolute path when invoking it. In zsh this would be

         alias gitbox=/home/xxx/src/gitbox/gitbox

3.   add any file or folder on your hard drive to gitbox with the command:

         gitbox add ~/.myconfigfile

4.   commit all the tracked files at once with a message containing the current
     date, with the command:

         gitbox push

5.   update the current repository with the command:

         gitbox pull

6.   when you move to a new computer, clone your gitbox repository, and just run

        gitbox install

    and all your files will appear in the right places via symlinks.
