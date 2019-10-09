 - history allows you to edit, recall, rerun previous commands
History ..
- rm is used to remove or delete directories, subdirectories, and all the files it contains. Data within the files is not destroyed, however the file is no longer accessible. 
Rm /home/.../… deletes the file by the pathname
Rm ./<file name> … deletes the file if it is in your current working directory
- mv is used to move one or more files/directories from one place to another
	Mv <file >  <folder/directory> .. moves the file.
	Mv <file> <file>.a … renames a file.
- Pwd is used to print the current working directory 
	It will print the full system path of the current directory 
- cp is used to copy files and directories.
Cp -a … archive files
Cp -f … force copy by removing the destination file if needed
Cp -r … copy an entire directory
Cp -i … prompts you before overwriting the file
- mkdir is used to create new directories (more than one directory can be specified). You can also create a parent directory with subdirectories 
	Mkdir [directory name] … create new in the current directory
	Mkdir ~/[directory name] … create new directory in home directory 
	Mkdir -p … create parent directories with multiple directories nested within
	Rmdir … removes a directory
- cd is used to change the current directory to the root folder. By default your terminal will take you to your home directory. You can also utilize cd to move around files. If you wanted to navigate a specific folder, you’d use the command ‘cd ~/<folder>’. If you unsure of your directories you can use the command ‘ls’ - which will list of all your files in the directory. Lastly, you can always command ‘cd ~’ to take you back to the home directory.
Cd ~ takes you back to the home directory 
Cd ~ …. Takes you to that specific folder
Cd - navigates previous directory
	Ls ~ list all  file names

