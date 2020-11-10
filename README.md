# dacco-cvs

DACCO was hosted in SourceForge and the files using CVS.

In order to keep the history of DACCO as close as possible I have pushed into this git repository the raw CVS repository from SourceForge.

This git repository is the "raw" files of the CVS compressed in gzip. The result of doing:
```sh
rsync -avv rsync://dacco.cvs.sourceforge.net/cvsroot/dacco/* .
find . -type f -exec gzip {} \;
```
And pushing it to git.

The reason of the gzip: certain files are bigger than 100 MB which is GitHub limit.
