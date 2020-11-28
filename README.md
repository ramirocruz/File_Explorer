# File_Explorer
* I have assumed the path to be space free
* We can avoid that by typing the path in quotes but I haven't implemented yet.

### The functions implemented are:
* There are two modes one is explorer mode (GUI mode) where you can view directories, scroll and open files in their default program.
* Second mode is the command mode by which we can perform  various operations.

### GUI mode:
* The explorer will assume the folder the program is run as the root directory, thus you cannot go to the parent of that directory.
* use up-down cursor and enter to navigate the directories or open a file.
* use left-right cursor to go to previous or forward locations like in a browser.
* use k-l keys to scroll next page of the directory. (If the total content in a directory are more than the screen size)
* use h key to go to home directory which is also the root.
* use `:` key to enter command mode.

### Command mode:
* User can now write some commands and see the result on the screen.
* The screen will show the file list as in gui mode.
* use `esc` key to got back to the gui mode.

#### List of commands:
* copy <source files> <destination directory>
* move <source files> <destination directory>
* rename <source file> <new name>
* create_file <filename> <destination directory>
* create_dir <dirname> <destination directory>
* delete_file <filepath>
* delete_dir <dirpath>
* goto <dirpath>  (similar to cd)
* search <dir/file name>  (give found/not found)
* The paths are of the format :
  * relative path to the current dir
  * absolute path starting with either `/` or `~/`

