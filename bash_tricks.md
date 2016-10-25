1. check folder size 

```bash
du -h foldername #more descriptive
du -hcs foldername #brief description
``` 
2. create softlink multiple files

```bash
pathDir="/path/to/directory/"
find $pathDir -name "*.format" -exec ln {} \;
# {} is whatever you find, and exec will execute a command for whatever you found. 
# \ is the full path to what was found 
```
3. go back to the previously visited directory 

```bash
cd "$OLDPWD"
```
4.To see the current progress in the server cpu

```bash
htop 
```
5. To see hidden file
```bash
less .git/config
```

6.Docker using as a nonroot user
If you would like to use Docker as a non-root user, you should now consider
adding your user to the "docker" group with something like:
```bash
sudo usermod -aG docker bohanni
```
Remember that you will have to log out and back in for this to take effect!
