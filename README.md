![Barney](http://media.giphy.com/media/12slK3kRc9ps08/giphy.gif)

### \#1 [ZSH](http://ohmyz.sh/)
![](http://i.imgur.com/l2JUuDU.jpg)
Thats a lie, we use the command line a lot

### \#2 [Dotfiles](https://github.com/duxilio/dotfiles)
![](http://m.memegen.com/undzf8.jpg)

### \#3 VIM
Check out [Matti's VIM docs](https://github.com/duxilio/command-line-awesomeness/VIM.md)

### \#4 Brace Expansion
```
cp /home/foo/realllylongname.cpp{,-old}
```
*Example Source: [user10767](http://stackoverflow.com/posts/68600/revisions)*

### \#5 Changing to the previous directory you were in
```
cd -
```

### \#6 Repeating the last command
```
!!
```
Most usefull in
```
sudo !!
```
*Example Source: [amrox](http://stackoverflow.com/posts/68429/revisions)*

### \#7 Replacing Typos
```
$ ehco foo bar baz
bash: ehco: command not found
$ ^ehco^echo
foo bar baz
```
*Example Source: [Seth](http://stackoverflow.com/users/8590)*

### \#8 Cursor Placement
1. `Alt + Click` lets you place your cursor by clicking
2. `Ctrl + A` moves your cursor to the beginning of the line
3. `Ctrl + C` cancels a command (duh)

### \#9 Piping Commands
Get the output of command A and use it as the input for command B. Example: List all files (including dotfiles using `-a`) and find a file which name contains `names`
```
ls -a | grep names
```

### \#10 Creating files
```
touch super-rad-kittens.html
```

### \#11 Creating/Appending to files
```
echo "contents of file" > filename.md
```
```
echo "appending this to file" >> filename.md
```

### \#12 Moving/Renaming Files/Folders
Use the `-R` flag for folders
```
mv current-filename.md new-filename.md
```

### \#13 Copying Files/Folders
Use the `-R` flag for folders
```
cp filename.md filename-2.md
```

### \#14 Awesomly Copying
In some (most actually) cases its super usefull to use `rsync` instead of `cp` when copying entire folders. This skips all files that are already in the destination and unchanged.
```
rsync ./ ~/path/to/dest/
```
[Super duper usefull for copying files to a server.](https://www.digitalocean.com/community/tutorials/how-to-use-rsync-to-sync-local-and-remote-directories-on-a-vps)
