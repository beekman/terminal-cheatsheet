# Terminal and Github Cheatsheet for Mac

_Letters are shown capitalized for readability only._
## SHORTCUTS

| Key/Command | Description |
| ----------- | ----------- |
| Ctrl + A   | Go to the beginning of the line you are currently typing on.  This also works for most text input fields system wide.  Netbeans being one exception |
| Ctrl + E   | Go to the end of the line you are currently typing on.  This also works for most text input fields system wide.  Netbeans being one exception |
| Ctrl + L   | Clears the Screen |
| Cmd + K    | Clears the Screen |
| Ctrl + U   | Cut everything backwards to beginning of line |
| Ctrl + K   | Cut everything forward to end of line |
| Ctrl + W   | Cut one word backwards using white space as delimiter |
| Ctrl + Y   | Paste whatever was cut by the last cut command |
| Ctrl + H   | Same as backspace |
| Ctrl + C   | Kill whatever you are running.  Also clears everything on current line |
| Ctrl + D   | Exit the current shell when no process is running, or send EOF to a the running process |
| Ctrl + Z   | Puts whatever you are running into a suspended background process. fg restores it |
| Ctrl + _   | Undo the last command. (Underscore.  So it's actually Ctrl + Shift + minus) |
| Ctrl + T   | Swap the last two characters before the cursor |
| Ctrl + F   | Move cursor one character forward |
| Ctrl + B   | Move cursor one character backward |
| Option + →  | Move cursor one word forward |
| Option + ←  | Move cursor one word backward |
| Esc + T  | Swap the last two words before the cursor |
| Esc + Backspace | Cut one word backwards using none alphabetic characters as delimiters |
| Tab  | Auto-complete files and folder names |

## CORE COMMANDS

| Key/Command | Description |
| ----------- | ----------- |
| cd [folder] | Change directory e.g. `cd Documents` |
| cd |  Home directory |
| cd ~ |  Home directory |
| cd /  | Root of drive |
| cd -  | Previous directory |
| ls | Short listing |
| ls -l | Long listing |
| ls -a | Listing incl. hidden files |
| ls -lh| Long listing with Human readable file sizes |
| ls -R | Entire content of folder recursively |
| sudo [command] | Run command with the security privileges of the superuser (Super User DO) |
| open [file] | Opens a file ( as if you double clicked it ) |
| top | Displays active processes. Press q to quit |
| nano [file] | Opens the file using the nano editor |
| vim [file] | Opens the file using the vim editor |
| clear |  Clears the screen |
| reset |  Resets the terminal display |

## CHAINING COMMANDS

| Key/Command | Description |
| ----------- | ----------- |
| [command-a]; [command-b] | Run command A and then B, regardless of success of A |
| [command-a] && [command-b] | Run command B if A succeeded |
| [command-a] \|\| [command-b] | Run command B if A failed |
| [command-a] & | Run command A in background |


## PIPING COMMANDS

| Key/Command | Description |
| ----------- | ----------- |
| [command-a] \| [command-b] | Run command A and then pass the result to command B e.g ps auxwww \| grep google |


## COMMAND HISTORY

| Key/Command | Description |
| ----------- | ----------- |
| history n |  Shows the stuff typed – add a number to limit the last n items |
| Ctrl + r  | Interactively search through previously typed commands |
| ![value] |  Execute the last command typed that starts with ‘value’ |
| ![value]:p |  Print to the console the last command typed that starts with ‘value’ |
| !! |  Execute the last command typed |
| !!:p |  Print to the console the last command typed |

## FILE MANAGEMENT

| Key/Command | Description |
| ----------- | ----------- |
| touch [file] |   Create a new file |
| pwd | Full path to working directory |
| . |  Current folder, e.g. `ls .` |
| .. | Parent/enclosing directory, e.g. `ls ..` |
| ls -l .. | Long listing of parent directory |
| cd ../../ | Move 2 levels up |
| cat | Concatenate to screen |
| rm [file] |  Remove a file, e.g. `rm data.tmp` |
| rm -i [file] | Remove with confirmation |
| rm -r [dir] | Remove a directory and contents |
| rm -f [file] | Force removal without confirmation |
| cp [file] [newfile] | Copy file to file |
| cp [file] [dir] | Copy file to directory |
| mv [file] [new filename] |  Move/Rename, e.g. `mv file1.ad /tmp` |
| pbcopy < [file] | Copies file contents to clipboard |
| pbpaste | Paste clipboard contents |
| pbpaste > [file] | Paste clipboard contents into file, `pbpaste > paste-test.txt` |

## DIRECTORY MANAGEMENT

| Key/Command | Description |
| ----------- | ----------- |
| mkdir [dir] | Create new directory |
| mkdir -p [dir]/[dir] |  Create nested directories |
| rmdir [dir] | Remove directory ( only operates on empty directories ) |
| rm -R [dir] | Remove directory and contents |
| less [file]|  Output file content delivered in screensize chunks |
| [command] > [file] |  Push output to file, keep in mind it will get overwritten |
| [command] >> [file] | Append output to existing file |
| [command] < [file] |  Tell command to read content from a file |

## SEARCH

| Key/Command | Description |
| ----------- | ----------- |
| find [dir] -name [search_pattern] | Search for files, e.g. `find /Users -name "file.txt"` |
| grep [search_pattern] [file] | Search for all lines that contain the pattern, e.g. `grep "Tom" file.txt` |
| grep -r [search_pattern] [dir] | Recursively search in all files in specified directory for all lines that contain the pattern |
| grep -v [search_pattern] [file] | Search for all lines that do NOT contain the pattern |
| grep -i [search_pattern] [file] | Search for all lines that contain the case-insensitive pattern |
| mdfind [search_pattern] | Spotlight search for files (names, content, other metadata), e.g. `mdfind skateboard` |
| mdfind -onlyin [dir] -name [pattern] | Spotlight search for files named like pattern in the given directory |

## HELP

| Key/Command | Description |
| ----------- | ----------- |
| [command] -h |  Offers help |
| [command] --help | Offers help |
| info [command] | Offers help |
| man [command] |  Show the help manual for [command] |
| whatis [command] | Gives a one-line description of [command] |
| apropos [search-pattern] | Searches for command with keywords in description |


## TERMINAL

| Key/Command | Description |
| ----------- | ----------- |
touch [file]|Create a new file
pwd|Full path to working directory
.|Current folder e.g. ls .
..|Parent/enclosing directory e.g. ls ..
ls -l ..|Long listing of parent directory
cd ../../|Move 2 levels up
cat|Concatenate to screen
rm [file]| Remove a file e.g. rm data.tmp
rm -i [file]|Remove with confirmation
rm -r [dir]|Remove a directory and contents
rm -f [file]|Force removal without confirmation
cp [file] [newfile]|Copy file to file
cp [file] [dir]|Copy file to directory
mv [file] [new filename]|Move/Rename e.g. mv file1.ad /tmp
pbcopy < [file]|Copies file contents to clipboard
pbpaste|Paste clipboard contents
pbpaste > [file]|Paste clipboard contents into file e.g. pbpaste > paste-test.txt

## DIRECTORY MANAGEMENT
| Key/Command | Description |
| ----------- | ----------- |
mkdir [dir]|Create new directory
mkdir -p [dir]/[dir]|Create nested directories
rmdir [dir]|Remove directory ( only operates on empty directories )
rm -R [dir]|Remove directory and contents
less [file]|Output file content delivered in screensize chunks
[command] > [file]|Push output to file, keep in mind it will get overwritten
[command] >> [file]|Append output to existing file
[command] < [file]|Tell command to read content from a file

## SEARCH
| Key/Command | Description |
| ----------- | ----------- |
|find [dir] -name [search_pattern]|Search for files e.g. find /Users -name file.txt|
grep [search_pattern] [file]|Search for all lines that contain the pattern e.g. grep "Tom" file.txt
grep -r [search_pattern] [dir]|Recursively search in all files in specified directory for all lines that contain the pattern
grep -v [search_pattern] [file]|Search for all lines that do NOT contain the pattern
grep -i [search_pattern] [file]|Search for all lines that contain the case-insensitive pattern
mdfind [search_pattern]|Spotlight search for files (names / content / other metadata) e.g. mdfind skateboard"
mdfind -onlyin [dir] -name [pattern]|Spotlight search for files named like pattern in the given directory

## HELP
| Key/Command | Description |
| ----------- | ----------- |
[command] -h|Offers help
[command] --help|Offers help
info [command]|Offers help
man [command]|Show the help manual for [command]
whatis [command]|Gives a one-line description of [command]
apropos [search-pattern]|Searches for command with keywords in description

## LESS
| Key/Command | Description |
| ----------- | ----------- |
j or ↓|scroll down by a line
 k or ↑|scroll up by a line
spacebar or Page Down|scroll down by a page
b or Page Up|scroll up by a page
q|quit

##Git Commits
| Key/Command | Description |
| ----------- | ----------- |
git add filename | adds filename to the commit
git add . | stages everything to the commit
git commit -m '*your commit message*'|Skips the commit message stage, using your commit message instead
git commit --amend|updates prior commit rather than creating a new commit
git diff|compare
git tag -a|Add a marker to the most recent commit. Append sha of commit to add tags later
git tag -d|Delete a tag
git branch|to list all branches
git branch *branch*|to create a new "footer-fix" branch
git branch -d *branch*|to delete the "footer-fix" branch
git checkout *branch*|switches to the branch
git revert <SHA-of-commit-to-revert>|takes the changes in a commit and does the exact opposite
| git pull |  pulls changes from the remote server and brings your local repo up to date.
git fetch | use when you have changes on both remote and local and you don't want to overwrite local changes.
git clone *URL* | create a new local repo cloning a remote repository
git push | sync the remote with your local commits
git merge | Merge the commits from the local and remote repositories

## GIT LOG
| Key/Command | Description |
| ----------- | ----------- |
git log --oneline|Each commit on one line
git log --stat|Shows github versioning info with each edit
git log -p|Prints the changes from each version to the console.
git shortlog | see how many commits each contributor has added to the repository
git shortlog -s -n| -s to show just the number of commits (rather than each commit's message) and -n to sort them numerically (rather than alphabetically by author name).
git log --author=*Bob* | filter down to the commits to the specified author (Bob)
git log --grep='*bug*' | filters down to the commits that reference the specified string (bug)


## GIT REMOTE
| Key/Command | Description |
| ----------- | ----------- |
git remote add| Add a remote connection.
git remote -v | See the details about a connection to a remote.
git remote add *upstream* https://url.com | adds a new remote connection with the shortname *upstream*
