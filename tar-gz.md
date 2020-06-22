# How to use ".tar.gz" files on Windows 10

**TL;DR**
1. Open PowerShell in your working folder
2. To decompress: tar -xvzf my_collection.tar.gz
3. To compress: tar -cvzf my_compressed_folder.tar.gz my_original_folder
4. To list the contents: tar -tvf my_collection.tar.gz

##Info:

".tar" files contain a collection of folders and files, in just a single file, but without applying any compression.
".tar.gz" files are ".tar" files that have been compressed using gzip.

## Syntax:

Syntax for decompress: 
tar [options] [the file that will be decompressed]
Syntax for compress:
tar [options] [the file that will be created] [the folder that will be compressed]

## Options:

The "tar" options:
-x : Extract archive
-c : Create archive
-v : Display verbose information
(About the -v option: If you are decompressing or compressing thousands of files, it would be better to omit this option because by displaying the name of every single file, the process will become slower).
-z : compress or decompress using gzip
(About the -z option: If you would like to create or extract a ".tar" file -i.e. without .gz extension at the end- then omit this option)
-f : The names of the files that will used for the process
-t : Display the contents of a ".tar.gz" archive, without extracting them.

## Example 1:

To decompress the file "my_file.tar.gz" which is inside the "outer_folder"
1. Open the "outer_folder" and point the mouse somewhere inside this folder, but not on a specific file
2. While pressing "Shift", right click the mouse and select "Open PowerShell Here"
3. In the PowerShell prompt type: tar -xvzf my_file.tar.gz
4. The file will be decompressed inside the "outer_folder"

## Example 2:

To compress the folder "my_folder" which is inside the "outer_folder"
1. Open the "outer_folder" and point the mouse somewhere inside the "outer_folder", but not on something specific
2. While pressing "Shift", right click the mouse and select "Open PowerShell Here"
3. In the PowerShell prompt type: tar -cvzf my_folder.tar.gz my_folder
4. The file my_folder.tar.gz will be created inside the "outer_folder"

## Example 3:

To display the folders and the files included in a ".tar.gz file", without extracting them:
tar -tf my_archive.tar.gz
Or, for more information:
tar -tvf my_archive.tar.gz

## Note:

Holding down the shift key and right clicking the mouse inside a folder, usually shows the option "Open PowerShell here" but depending on the configuration it may show the option "Open Command window here". Nevertheless, both PowerShell and Command prompt can be used to handle .tar.gz files.
If though no options appear in the menu, then on the address bar which appears at the top of the opened folder, just type: powershell, or if you prefer the command prompt then type: cmd, and press enter. In this case, no path is needed and only the words powershell or cmd should be written in the address bar.
Also, to properly exit from powershell or cmd, just type: exit

## Important:

When decompressing or compressing files, make sure that inside your working folder there are no other items with the same name as the name of the items that will be created, otherwise the new items will automatically replace the old ones, without any warning and without moving the old ones to the recycle bin.
Notice also that a ".tar.gz" may extract several folders and files, into your working folder, and not necessarily only one folder. So, to be on the safe side, it would be better to create a new folder and to extract the files inside that folder.
