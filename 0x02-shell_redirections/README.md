This is where I will describe what each script for the 0x02 project is doing.

0. A script that prints "hello world" followed by a new line to the standard output
echo "Hello, World"
1. script that displays a confused smiley
echo "\"(Ôo)'"
2. display the content of the /etc/passwd file
less /etc/passwd
3. display the content of /etc/passwd and /etc/hosts
cat /etc/passwd /etc/hosts
4. display the last 10 lines of a /etc/passwd
tail /etc/passwd
5. display the first 10 lines of /etc/passwd
head /etc/passwd
6. displays third line of file
head -3 ./iacta | tail +3
7. create a file with a crazy file name full of special characters not to be treated as special characters
echo "Best School" > \\*\\\\\'\""Best School"\"\\\'\\\\*$\\?\\*\\*\\*\\*\\*:\)
8. a script that redirects the output of ls -la into a file
ls -la > ls_cwd_content
9. a script that duplicates the last line of a file
tail -1 ./iacta >> ./iacta
10. delete files with .js extension that are present in the current directory and its subfolders
find *.js -delete
11. a script that counts the nubmer of directories and subdirectories (current and parent directories not counted, hidden directories counted)
find ./* -type d | wc -l
12.Create a script that displays the 10 newest files in the current directory.
ls -1t | head
13. Create a script that takes a list of words as input and prints only words that appear exactly once.
sort | uniq -u
14. Display lines containing the pattern “root” from the file /etc/passwd
grep "root" /etc/passwd
15. Display the number of lines that contain the pattern “bin” in the file /etc/passwd
grep "bin" /etc/passwd | wc -l
16.Display lines containing the pattern “root” and 3 lines after them in the file /etc/passwd.
grep "root" -3 /etc/passwd
17. Display all the lines in the file /etc/passwd that do not contain the pattern “bin”.
grep -v "bin" /etc/passwd
18.Display all lines of the file /etc/ssh/sshd_config starting with a letter.
grep -i "^[a-z]" /etc/ssh/sshd_config
19.Replace all characters A and c from input to Z and e respectively.
tr 'Ac' 'Ze'
20.Create a script that removes all letters c and C from input.
tr -d Cc
21.Write a script that reverse its input.
rev
22.Write a script that displays all users and their home directories, sorted by users.
cut -d: -f1,6 /etc/passwd | sort



