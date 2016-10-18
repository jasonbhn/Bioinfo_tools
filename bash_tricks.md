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
3. 
