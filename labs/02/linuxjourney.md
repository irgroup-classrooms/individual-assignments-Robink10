

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
Robin@LAPTOP-SLKJPVJT MINGW64 ~ (first_branch)
$ mkdir source_dir
touch source_dir/file1.txt source_dir/file2.txt source_dir/file3.txt

Robin@LAPTOP-SLKJPVJT MINGW64 ~ (first_branch)
$ mkdir target_dir

Robin@LAPTOP-SLKJPVJT MINGW64 ~ (first_branch)
$ cp -n source_dir/* target_dir/

Robin@LAPTOP-SLKJPVJT MINGW64 ~ (first_branch)
$ ls target_dir/
file1.txt  file2.txt  file3.txt
```
```
11.mv
Robin@LAPTOP-SLKJPVJT MINGW64 ~ (first_branch)
$ touch example.txt

Robin@LAPTOP-SLKJPVJT MINGW64 ~ (first_branch)
$ mv example.txt renamed_example.txt

Robin@LAPTOP-SLKJPVJT MINGW64 ~ (first_branch)
$ mv renamed_example.txt target_dir/

Robin@LAPTOP-SLKJPVJT MINGW64 ~ (first_branch)
$ ls target_dir/
file1.txt  file2.txt  file3.txt  renamed_example.txt
```
```
12.mkdir
Robin@LAPTOP-SLKJPVJT MINGW64 ~ (main)
$ mkdir dir1 dir2

Robin@LAPTOP-SLKJPVJT MINGW64 ~ (main)
$ touch file1.txt file2.txt file3.txt

Robin@LAPTOP-SLKJPVJT MINGW64 ~ (main)
$ mv file1.txt dir1/
mv file2.txt dir1/
mv file3.txt dir2/

Robin@LAPTOP-SLKJPVJT MINGW64 ~ (main)
$

Robin@LAPTOP-SLKJPVJT MINGW64 ~ (main)
$ ls dir1
file1.txt  file2.txt

Robin@LAPTOP-SLKJPVJT MINGW64 ~ (main)
$ ls dir 2
ls: cannot access 'dir': No such file or directory
ls: cannot access '2': No such file or directory

Robin@LAPTOP-SLKJPVJT MINGW64 ~ (main)
$ ls dir2
file3.txt

```
```
13.remove
Robin@LAPTOP-SLKJPVJT MINGW64 ~ (first_branch)
$ touch ./-file
Robin@LAPTOP-SLKJPVJT MINGW64 ~ (first_branch)
$ rm ./-file
```
```
14.find
Robin@LAPTOP-SLKJPVJT MINGW64 ~ (first_branch)
$ find / -type f -name "*net*"
/bin/core_perl/libnetcfg
/bin/msys-nettle-8.dll
/bin/nettle-hash.exe
/bin/nettle-lfib-stream.exe
/bin/nettle-pbkdf2.exe
/etc/networks
/mingw64/bin/libnettle-8.dll
/mingw64/lib/tcl8.6/tzdata/Asia/Novokuznetsk
/mingw64/libexec/git-core/libnettle-8.dll
/usr/bin/core_perl/libnetcfg
/usr/bin/msys-nettle-8.dll
/usr/bin/nettle-hash.exe
/usr/bin/nettle-lfib-stream.exe
/usr/bin/nettle-pbkdf2.exe
/usr/share/gnupg/sks-keyservers.netCA.pem
/usr/share/gtk-doc/html/p11-kit/trust-glib-networking.html
/usr/share/perl5/core_perl/Net/netent.pm
/usr/share/perl5/vendor_perl/Mail/Internet.pm
/usr/share/perl5/vendor_perl/URI/telnet.pm
/usr/share/vim/vim91/autoload/netrw.vim
/usr/share/vim/vim91/autoload/netrwFileHandlers.vim
/usr/share/vim/vim91/autoload/netrwSettings.vim
/usr/share/vim/vim91/autoload/netrw_gitignore.vim
/usr/share/vim/vim91/compiler/dotnet.vim
/usr/share/vim/vim91/doc/netbeans.txt
/usr/share/vim/vim91/doc/pi_netrw.txt
/usr/share/vim/vim91/ftplugin/jsonnet.vim
/usr/share/vim/vim91/ftplugin/netrc.vim
/usr/share/vim/vim91/ftplugin/xinetd.vim
/usr/share/vim/vim91/indent/xinetd.vim
/usr/share/vim/vim91/keymap/bulgarian-phonetic.vim
/usr/share/vim/vim91/keymap/sinhala-phonetic_utf-8.vim
/usr/share/vim/vim91/keymap/thaana-phonetic_utf-8.vim
/usr/share/vim/vim91/plugin/netrwPlugin.vim
/usr/share/vim/vim91/syntax/netrc.vim
/usr/share/vim/vim91/syntax/netrw.vim
/usr/share/vim/vim91/syntax/snnsnet.vim
/usr/share/vim/vim91/syntax/xinetd.vim
/usr/share/vim/vim91/tools/vim_vs_net.cmd
/proc/net/if_inet6
/proc/registry/HKEY_CLASSES_ROOT/.URL/OpenWithProgIds/InternetShortcut
```
```
15.help
Robin@LAPTOP-SLKJPVJT MINGW64 ~ (main)
$ help echo
echo: echo [-neE] [arg ...]
    Write arguments to the standard output.

    Display the ARGs, separated by a single space character and followed by a
    newline, on the standard output.

    Options:
      -n        do not append a newline
      -e        enable interpretation of the following backslash escapes
      -E        explicitly suppress interpretation of backslash escapes

    `echo' interprets the following backslash-escaped characters:
      \a        alert (bell)
      \b        backspace
      \c        suppress further output
      \e        escape character
      \E        escape character
      \f        form feed
      \n        new line
      \r        carriage return
      \t        horizontal tab
      \v        vertical tab
      \\        backslash
      \0nnn     the character whose ASCII code is NNN (octal).  NNN can be
                0 to 3 octal digits
      \xHH      the eight-bit character whose value is HH (hexadecimal).  HH
                can be one or two hex digits
      \uHHHH    the Unicode character whose value is the hexadecimal value HHHH.
                HHHH can be one to four hex digits.
      \UHHHHHHHH the Unicode character whose value is the hexadecimal value
                HHHHHHHH. HHHHHHHH can be one to eight hex digits.

    Exit Status:
    Returns success unless a write error occurs.

Robin@LAPTOP-SLKJPVJT MINGW64 ~ (main)
$ help logout
logout: logout [n]
    Exit a login shell.

    Exits a login shell with exit status N.  Returns an error if not executed
    in a login shell.

Robin@LAPTOP-SLKJPVJT MINGW64 ~ (main)
$ help pwd
pwd: pwd [-LPW]
    Print the name of the current working directory.

    Options:
      -L        print the value of $PWD if it names the current working
                directory
      -P        print the physical directory, without any symbolic links
      -W        print the Win32 value of the physical directory

    By default, `pwd' behaves as if `-L' were specified.

    Exit Status:
    Returns 0 unless an invalid option is given or the current directory
    cannot be read.
```
```
16.man
Der man Befehl ist standartmäßig nicht heruntergeladen und muss mit einem Zusatzt heruntergeladen werden. Ich habe help als Alternative benutzt.
Robin@LAPTOP-SLKJPVJT MINGW64 ~ (main)
$ ls --help
Usage: ls [OPTION]... [FILE]...
List information about the FILEs (the current directory by default).
Sort entries alphabetically if none of -cftuvSUX nor --sort is specified.

Mandatory arguments to long options are mandatory for short options too.
  -a, --all                  do not ignore entries starting with .
  -A, --almost-all           do not list implied . and ..
      --author               with -l, print the author of each file
  -b, --escape               print C-style escapes for nongraphic characters
      --block-size=SIZE      with -l, scale sizes by SIZE when printing them;
                               e.g., '--block-size=M'; see SIZE format below
  -B, --ignore-backups       do not list implied entries ending with ~
  -c                         with -lt: sort by, and show, ctime (time of last
                               modification of file status information);
                               with -l: show ctime and sort by name;
                               otherwise: sort by ctime, newest first
  -C                         list entries by columns
      --color[=WHEN]         colorize the output; WHEN can be 'always' (default
                               if omitted), 'auto', or 'never'; more info below
  -d, --directory            list directories themselves, not their contents
  -D, --dired                generate output designed for Emacs' dired mode
  -f                         do not sort, enable -aU, disable -ls --color
  -F, --classify             append indicator (one of */=>@|) to entries
      --file-type            likewise, except do not append '*'
      --format=WORD          across -x, commas -m, horizontal -x, long -l,
                               single-column -1, verbose -l, vertical -C
      --full-time            like -l --time-style=full-iso
  -g                         like -l, but do not list owner
      --group-directories-first
                             group directories before files;
                               can be augmented with a --sort option, but any
                               use of --sort=none (-U) disables grouping
  -G, --no-group             in a long listing, don't print group names
  -h, --human-readable       with -l and -s, print sizes like 1K 234M 2G etc.
      --si                   likewise, but use powers of 1000 not 1024
  -H, --dereference-command-line
                             follow symbolic links listed on the command line
      --dereference-command-line-symlink-to-dir
                             follow each command line symbolic link
                               that points to a directory
      --hide=PATTERN         do not list implied entries matching shell PATTERN
                               (overridden by -a or -A)
      --hyperlink[=WHEN]     hyperlink file names; WHEN can be 'always'
                               (default if omitted), 'auto', or 'never'
      --indicator-style=WORD  append indicator with style WORD to entry names:
                               none (default), slash (-p),
                               file-type (--file-type), classify (-F)
  -i, --inode                print the index number of each file
  -I, --ignore=PATTERN       do not list implied entries matching shell PATTERN
  -k, --kibibytes            default to 1024-byte blocks for disk usage;
                               used only with -s and per directory totals
  -l                         use a long listing format
  -L, --dereference          when showing file information for a symbolic
                               link, show information for the file the link
                               references rather than for the link itself
  -m                         fill width with a comma separated list of entries
  -n, --numeric-uid-gid      like -l, but list numeric user and group IDs
  -N, --literal              print entry names without quoting
  -o                         like -l, but do not list group information
  -p, --indicator-style=slash
                             append / indicator to directories
  -q, --hide-control-chars   print ? instead of nongraphic characters
      --show-control-chars   show nongraphic characters as-is (the default,
                               unless program is 'ls' and output is a terminal)
  -Q, --quote-name           enclose entry names in double quotes
      --quoting-style=WORD   use quoting style WORD for entry names:
                               literal, locale, shell, shell-always,
                               shell-escape, shell-escape-always, c, escape
                               (overrides QUOTING_STYLE environment variable)
  -r, --reverse              reverse order while sorting
  -R, --recursive            list subdirectories recursively
  -s, --size                 print the allocated size of each file, in blocks
  -S                         sort by file size, largest first
      --sort=WORD            sort by WORD instead of name: none (-U), size (-S),
                               time (-t), version (-v), extension (-X)
      --time=WORD            change the default of using modification times;
                               access time (-u): atime, access, use;
                               change time (-c): ctime, status;
                               birth time: birth, creation;
                             with -l, WORD determines which time to show;
                             with --sort=time, sort by WORD (newest first)
      --time-style=TIME_STYLE  time/date format with -l; see TIME_STYLE below
  -t                         sort by time, newest first; see --time
  -T, --tabsize=COLS         assume tab stops at each COLS instead of 8
  -u                         with -lt: sort by, and show, access time;
                               with -l: show access time and sort by name;
                               otherwise: sort by access time, newest first
  -U                         do not sort; list entries in directory order
  -v                         natural sort of (version) numbers within text
  -w, --width=COLS           set output width to COLS.  0 means no limit
  -x                         list entries by lines instead of by columns
  -X                         sort alphabetically by entry extension
  -Z, --context              print any security context of each file
  -1                         list one file per line.  Avoid '\n' with -q or -b
      --append-exe           append .exe if cygwin magic was needed
      --help     display this help and exit
      --version  output version information and exit

The SIZE argument is an integer and optional unit (example: 10K is 10*1024).
Units are K,M,G,T,P,E,Z,Y (powers of 1024) or KB,MB,... (powers of 1000).
Binary prefixes can be used, too: KiB=K, MiB=M, and so on.

The TIME_STYLE argument can be full-iso, long-iso, iso, locale, or +FORMAT.
FORMAT is interpreted like in date(1).  If FORMAT is FORMAT1<newline>FORMAT2,
then FORMAT1 applies to non-recent files and FORMAT2 to recent files.
TIME_STYLE prefixed with 'posix-' takes effect only outside the POSIX locale.
Also the TIME_STYLE environment variable sets the default style to use.

Using color to distinguish file types is disabled both by default and
with --color=never.  With --color=auto, ls emits color codes only when
standard output is connected to a terminal.  The LS_COLORS environment
variable can change the settings.  Use the dircolors command to set it.

Exit status:
 0  if OK,
 1  if minor problems (e.g., cannot access subdirectory),
 2  if serious trouble (e.g., cannot access command-line argument).

GNU coreutils online help: <https://www.gnu.org/software/coreutils/>
Report any translation bugs to <https://translationproject.org/team/>
Full documentation <https://www.gnu.org/software/coreutils/ls>
or available locally via: info '(coreutils) ls invocation'
```
```
17.whatis
extiert auch nicht
```
```
18.alias
Robin@LAPTOP-SLKJPVJT MINGW64 ~ (main)
$ alias gs='git status'

Robin@LAPTOP-SLKJPVJT MINGW64 ~ (main)
$ alias
alias gs='git status'
alias ll='ls -l'
alias ls='ls -F --color=auto --show-control-chars'
alias winget='winpty winget.exe'

Robin@LAPTOP-SLKJPVJT MINGW64 ~ (main)
$ unalias gs

Robin@LAPTOP-SLKJPVJT MINGW64 ~ (main)
$
```
```
19. Programm schließt
```







