https://www.terminaltemple.com/ open this to work on linux commands

1. pwd = present working directory or print working directory

2. ls = list of all folders in present directory 

3. ls -a = lists all hidden files startign with . along with all folders
   in linus any file starting with . is considered hidden file like 
  .file1
  .config
  .bashrc
  .gitignore

  Why are files hidden?

  Hidden files are usually used to store:
  Configuration settings , System preferences , Application data

  For example:
  .bashrc → stores terminal settings
  .config → app configurations
  .git → Git repository data

  🔹 Why not show them normally?

  Because:
  They are not needed for everyday use
  Showing them would clutter the screen
  They are often important system files (accidental changes can break things)

  ls -a shows
  normal files ✅
  hidden files ✅
  also . (current directory)
  and .. (parent directory)

4. mkdir = make directory : mkdit myFolder
 
5. cd = change directory , changes directory : cd myFodler , cd ..

6. touch = used to make new files : touch file1.txt

7. echo "hello" = displays hello : echo"hello" > file1.ttx ( writes hello in file1)

8. cat = displays content of file : cat file1.txt

9. wc = wprd count : wc file.txt

10. cp = copy file/ directory : cp file1.txt copy.txt

11. mv = move or rename file : mv file1.txt new.txt

12. ls -l = long listing : permision , time edited and many more things 

13. tree = shows fodler in tree format ( nested jaisa )  
    tree are not supoorted in oniline kernels , and can be installed in system only using sudo apt install tree

14. date : Mon Apr 13 18:53:50 2026

15. whoami : saransh/saran gives your name no matter in whichever folder u r

16. df -h = displays disk sapce in human readable format in gb/mb
    cmd doesnt support it as it a unix cammand and is supported in linux and macos

17. rm = removes file permanently : rm file1.txt

18. rmdir = remove directory : rmdir folderName

19. nano = Open / Create a file : nano file.txt

    If file exists → opens it
    If not → creates new file

    Write content
    Just start typing:

    Hello world
    This is nano

    again like tree , ony i unix command line , not supported in online env

20. less = less is a command used to view file contents page by page : less file.txt

    cat	                              less
    Shows full content               	Page by page
    Not good for large files	        Best for large files

21. head Displays the first few lines of a file. : head -n 5 file.txt :tail -5 file.txt ( default = 10 ) : head file.txt
22. tail Displays the last few lines of a file. : tail -n 5 file.txt : tail -5 file.txt ( default = 10 ) : tail file.txt

23. grep = Global Regular Expression Print ; searches words , patterns in file : grep "hello" file.txt

24. wc -l = counts no of lines : wc -l file.txt

25. chmod = change file permission for all : chmod 777 file1.txt
     
    777 means alll have all permissions 
    owner u , grp g , others o 
    4 = read (R ), 2 write (w) , 1 execute (x)
    766 , rwx , rw , rw
    chmod u+x file.txt : execute permission given to user/owner
    chmod g-w file.txt : write permission removed from grp

    check permission :-
    ls -l
    -rwxr-xr--

    rwx , r-x  , r--
    rwx → user
    r-x → group
    r-- → others

26. ps = used to see process status which all process are running 
27. ps -e = all system processes  

28. echo $$ = echo $$ is used to display the process ID of the current shell.
    
    A shell variable is a variable used in the Linux shell (terminal) to store data.

29. uptime : 
    
    10:30:25 up 2:15,  1 user,  load average: 0.10, 0.20, 0.30
    current time , up time , user , load in 1 5 15 min

30. free -h : free → shows memory usage (RAM) , -h → human-readable (MB/GB)

                  total   used   free   shared  buff/cache  available
    Mem:          8.0G   3.2G   1.5G    200M     3.3G        4.2G
    Swap:         2.0G   0.5G   1.5G

    | Column     | Meaning             |
    | ---------- | ------------------- |
    | total      | Total RAM           |
    | used       | RAM being used      |
    | free       | Completely free RAM |
    | shared     | Shared memory       |
    | buff/cache | Cached memory       |
    | available  | Usable memory       |

31. lscpu = List CPU : It is used to display CPU (processor) information

32. who

    user1   pts/0   2026-04-13 10:20
    user2   pts/1   2026-04-13 10:25

    | Field     | Meaning          |
    | --------- | ---------------- |
    | user1     | Username         |
    | pts/0     | Terminal session |
    | date/time | Login time       |
33. sort file.txt = sorts lines in acc to alphabets

34. man = man command is used to display the manual or help page of a command in Linux.

    man ls   ✅
    man grep ✅

    man ls grep ❌

    man 5 passwd 
    
    Here:
    5 = section number
    passwd = topic

35. clear adn exit