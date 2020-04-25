# ls.c
We need to specify the correct directory name to get the name of the files present in the directory. 

#ALGORITHM 
 
1. Start the process. 
2. Create a directory entry using dirent structure. 
3. To define a pointer to a structure, dp predefined structure DIR and another pointer to a structure called ep. 
4. The directory is opened using the opendir() function. 
5. In the while loop read each entry using the readdir() function which returns a pointer. 
6. If no pointer is returned the program is exited, else it will list the files inside the directory. 
7. The closedir() function closes this open directory.Input source path to list all files and sub-directories. Store it in some variable say path. 
8. Open directory stream using opendir() and store its reference to *dir of DIR type. 
9. Initialize another variable of pointer to structure dirent type, say struct dirent *dp. 
10. Read next element from directory stream using dp = readdir(dir). 
11. Print current directory stream item name, using dp->name. 
12. Repeat step 4-5 till dp != NULL. 
13. Finally, close the directory stream pointed by dir variable. 
14. Stop the process. 
