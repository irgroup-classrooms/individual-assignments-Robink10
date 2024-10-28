

```
1. The Shell
Exercises

Try some other Linux commands and see what they output:

    $ date
    $ whoami

Robin@LAPTOP-SLKJPVJT MINGW64 ~
$ date
Mon Oct 28 19:37:46     2024

Robin@LAPTOP-SLKJPVJT MINGW64 ~
$ whoami
Robin
```
```


3. cd (Change Directory)
Exercises

    Run the cd command without any flags, where does it take you?

Robin@LAPTOP-SLKJPVJT MINGW64 ~/dis08
$ cd

lenna@Lennard MINGW64 ~
$
```
```
4. ls (Liste Directories)
Exercises

Run ls with different flags and see the output you receive.

    ls -R: recursively list directory contents
    ls -r: reverse order while sorting
    ls -t: sort by modification time, newest first
```
```
5. touch
Exercises

    Create a new file
    Note the timestamp
    Touch the file and check the timestamp once again
Robin@LAPTOP-SLKJPVJT MINGW64 ~
$ touch mysuperduperfile
```
```
6. file
Exercises

Run the file command on a few different directories and files and note the output.
```
```
7. cat
Exercises

Run cat on different files and directories. Then try to cat multiple files.
```
```
8. less
q - Used to quit out of less and go back to your shell.
Page up, Page down, Up and Down - Navigate using the arrow keys and page keys.
g - Moves to beginning of the text file.
G - Moves to the end of the text file.
/search - You can search for specific text inside the text document. Prefacing the words you want to search with /
h - If you need a little help about how to use less while you’re in less, use help.
```
```
9. history
Robin@LAPTOP-SLKJPVJT MINGW64 ~
$ !!
history
    1  pwd
    2  is
    3  Is
    4  ls
    5  cd tools
    6  is -1
    7  cd tools
    8  mkdir dis08
    9  cd dis08
   10  touch notes.txt
   11  Is
   12  is notes.txt
   13  Is notes.txt
   14  echo "hello world" > notes.txt
   15  cd
   16  cat notes.txt dir_overview
   17  touch notes.txt
   18  Is
   19  ls
   20  pwd
   21  mkdir dis08
   22  cd dis08
   23  touch notes.txt
   24  ls
   25  echo "hello world" > notes.txt
   26  cat notes.txt
   27  ls > dir_overview.txt
   28  cat dir_overview.txt
   29  rm notes.txt
   30  ls
   31  history
   32  cp dir_overview.txt dir_overview_backup.txt
   33  ls
   34  mv dir_overview_backup.txt dir_overview_copy.txt
   35  ls
   36  cd ...
   37  rm -rf dis08
   38  echo hello world
   39  date
   40  whoami
   41  ls -R
   42  ls -r
   43  rm -rf dis08
   44  rm -rf dis08
   45  pwd
   46  cd ..
   47  rm rf- dis08
   48  rm -rf dis08
   49  touch newfile
   50  touch mysuperduperfile
   51  -l
   52  ls -l
   53  file banan.jpg
   54  date
   55  whoami
   56  cat
   57  less "C:\Users\Robin\Documents\TH-Köln\Semester_3\DIS08_DatenmodellierungData_Modelling\829-0.txt"
   58  histroy
   59  history
   60  history
   61  history
   62  history
```
```
10. cp (Copy)





