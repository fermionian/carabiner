### How to add local packages with conda ###

espeically when you don't want to write a conda package...

Conda does not want you add PYTHONPATH, as it messed up with the environment control. 

Add a .pth file to the directory $HOME/path/to/anaconda/lib/pythonX.X/site-packages. 

This can be named anything (it just must end with .pth). A .pth file is just a newline-separated listing of the full path-names of directories that will be added to your path on Python startup.

From: [Anaconda: Permanently include external packages (like in PYTHONPATH)](https://stackoverflow.com/questions/37006114/anaconda-permanently-include-external-packages-like-in-pythonpath/37008663)

