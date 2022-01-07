Below are a list of scripts --> and what they do with the commands used to write the script beneath
0-current_working_directoy --> prints the absolute path name of the current working directoy
pwd
1-listit --> displays the contents list of your current directory
ls
2-bring_me_home --> changes the working directory to user's home directory
cd ~root
3-listfiles --> displays current directory contents in long format
ls -l
4-listmorefiles --> display current directory contents, including hidden files using long format
ls -la
5-listfilesdigitonly --> display current directory contents in long format with user and group IDs displayed numerically
ls -lan
6-firstdirectory --> creates a directory named my_first_directory in the /tmp/ directory
mkdir /tmp/my_first_directory
7-movethatfile --> moves the file betty from /tmp/ to /tmp/my_first_directory
mv /tmp/betty /tmp/my_first_directory
8-firstdelete --> deletes the file betty
rm /tmp/my_first_directory/betty
9-firstdirdeletion --> deletes the directory my_first_directory that is in the /tmp directory
rm -r /tmp/my_first_directory
10-back --> changes the working directory to the previous one
cd -
11-lists --> lists all files even the hidden ones in the current directory and the parent of the working directory and the /boot directory in long format
ls -la . .. /boot
12-file_type --> prints the type of file name iamafile
file /tmp/iamafile
13-symbolic_link --> creates a symbolic link to /bin/ls names __ls__
ln -s /bin/ls __ls__
14-copy_html --> copies all the HTML files from the current working directory tot he parent of the working diretory but only files that did not exist in the parent or were newer than the version in the parent of the working diretory
cp -u *html

end of scripts and the commands that make them up. 