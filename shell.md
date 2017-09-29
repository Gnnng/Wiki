Cheatsheet
=========

find
------

To change all the directories to 755 (`drwxr-xr-x`):

```
find sampledir -type d -exec chmod 755 {} \;
```

To change all the files to 644 (`-rw-r--r--`):

```
find sampledir -type f -exec chmod 644 {} \;
```

entr
------

Install via `sudo apt install entr`.

Watch a directory and compile upon any changes:

```
ls -d sampledir/* | entr sh -c "make && make test"
```

autossh
---------

Keep ssh session alive. Install via `sudo apt install autossh`

Better to alias it with:

```
alias assh='autossh -M `python -c "import random; print random.randint(60000, 65000)"`'
```

wget
----------

Download all listed files on a web page (HTTP File Server)

```
wget --mirror --no-parent http://yoururl
```

tmux
---------

Attach to a named session, or create one in advance before attaching if none exists

```
tmux new -As mysession
```


