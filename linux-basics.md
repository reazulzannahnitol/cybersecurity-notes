## MUST KNOW KALI TERMINAL COMMANDS:
ctrl+alt+T - open terminal
ctrl+shift+T - new tab terminal
ctrl+shift+W - close tab terminal
clear - clear all commands (After clearing if we keep clicking up arrow we can see old commands)
sudo apt update - see what updates are available
sudo apt upgrade - install those updates
ctrl+c - to cancel or get out of running command
q - quit from something
pwd - print working directory (current location)
ls - we can see how many files and folder in our current location
ls foldername - show all file and folder in that folder
~ - takes to home directory
/ - takes to root directory
cd desktop - with cd we can go to any folder typing folder name
cd .. - go back 1 folder
../ - go back 1 folder
../.. - go back 2 folder (more .. means more back folder)
mkdir - make a new folder
touch - for creating file
cat nt.txt - check what is inside text file
cat > filename - create a text file
cat >> add some text at end - appending text at end (ctrl+D to go back to command)
echo "hello world" - it prints texts 
echo "Hello" >> nt.txt - add some texts in a text file
echo "Hello" > nt.txt - replace completely texts in a text file
nano nt.txt - we can use this text file as text file right inside terminal (ctrl+O) to save and then (ctrl+x) to exit nano
mousepad - open a text editor outside of terminal like notepad
./filename.txt - to run or execute a file or script
bash filename.txt - can run or execute a script without permission
less filename.txt - view file page by page (q to quit) (/ to find something, n for next of that searched keyword, q to quit)
head filename.txt - read first 10 lines
tail filename.txt - read last 10 lines
tail -n +507 /etc/snort/snort.conf | head -n 6  - start from line 507 and end at 512 line
head -20 filename.txt - read first 20 lines (same for tail)
batcat filename.txt - read lines with number
history - show all command history
whatis - tells which command is what
whoami - show current logged-in user
id - display user identity information
ifconfig or ip a - show ip and all other network details
ping websitename.com - check network or pulse of a website
df -h - check disk space
grep keyword filename.txt - search for text inside a file (case sensitive)
kali >cat /etc/snort/snort.conf | grep output - in snort file we will get result only with lines who has word 'output'
find filename - find a file
cp source destination- copy file
mv source destination - move file
mv nit.txt ev.txt - rename file
rm nit.txt - remove file
rmdir foldername or rm -r foldername - delete a folder
passwd - change linux password
man aircrack-ng - see manual of a command
aircrack-ng -h or aircrack-ng --help - see list of different command options(some work with, -h some with --help)

locate - locate will search through entire database (might not find things that just created because it uses database that updated once a day
sudo updatedb - Update database
whereis - find binary files and it's manual page if available
PATH VARIABLE - A list of directories where executable files are usually located. Common directories include `/usr/bin` and `/usr/sbin`. example: echo $PATH
which - returns the location of only the binary. example: which aircrack-ng
find - Searches for files and directories in specified location and its subdirectories by user based on name, type, size, etc. Example: find / -type f -name apache2
grep - searches for keyword or specific text inside files or command output. example: grep "school" buildings.txt    example: ps aux | grep apache2 (searching if apache2 service is running)
ps aux - can see all proccesses that are running in the machine
