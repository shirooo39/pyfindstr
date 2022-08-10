# pyfindstr
pyfindstr is just a simple Python script that looks up for a keyword on any files (or specified by the file type) and recursively.  

<img style="width: 65%;" src="https://user-images.githubusercontent.com/38461122/183863502-69cf376c-f456-4e7e-adcc-99ab23c5a759.png" atl="screenshot of pyfindstr"></img>

(You could also say that this is just a fancy way to look up for a string in a file. ¯\_( ツ )_/¯)

## Usage
You need to have Python (at least version 3.5 or higher) installed first on your system.  
Then, it's as simple as this:
- Open up your command prompt or terminal.
- Type in ```python findstry.py```

The same can be achieved on Windows by using this command:
``` Batch
findstr /s /i "(keyword)" "(path)"
```

For example:
``` Batch
findstr /s /i "cdn" "D:\Projects\GitHub\Shiro39\jekyll-mdui\*.html"
```
This command will look up for the keyword cdn on any .html files in the given path.  
Feel free to read more about the findstr command [in here](https://ss64.com/nt/findstr.html).

BUT! this script does NOT use any of the OS' native command. ```pathlib``` is the one that does the magic in this script.
