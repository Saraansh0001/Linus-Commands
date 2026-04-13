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

4. 