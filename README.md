# Linux
ls - list the files and directories in the current directory
ls 

cd - change the current directory
cd dir_name

mkdir - create a new directory
mkdir rohan

rmdir - remove a directory
rmdir rohan

pwd - print the current working directory
pwd

cp - copy files or directories
#We will copy a file called example.txt from the current directory to a directory called backup
cp example.txt backup/

mv - move or rename files or directories
mv example.txt backup/

rm - remove files or directories
rm example.txt

touch - create a new empty file or update the timestamp of an existing file
touch shayan.txt

cat - concatenate and display files
cat example.txt

man - manual for a command
man ls

htop - an interactive process viewer and system monitor
htop

chmod - change the permissions of a file or directory
# The first digit represents the owner of the file/directory
# The second digit represents the group that the file/directory belongs to
# The third digit represents all other users
# 0 (no permission)
# 1 (execute only)
# 2 (write only)
# 3 (write and execute)
# 4 (read only)
# 5 (read and execute)
# 6 (read and write)
# 7 (read, write, and execute) 


chmod 700 file.txt
chown - change the owner of a file or directory
chown new_owner example.txt

tar - create or extract compressed archive files
# x: extract files from an archive
# t: list the contents of an archive
# r: append files to an existing archive
# z: use gzip compression
# j: use bzip2 compression
# cf: create file
#xf: extract file
tar cf archive.tar file1 file2 file3

gzip - compress files

gzip file.txt

gunzip - decompress compressed files

gunzip file.txt.gz

ssh - connect to a remote server securely

ssh username@server_address

scp - securely copy files between systems
scp myfile.txt user@remotehost:/home/user/

ping - test network connectivity
ping 8.8.8.8

ifconfig - display or configure network interfaces
ifconfig

netstat - display network connection information
netstat

route - view or configure network routing tables
route [options] [add/delete/show]

top - display system resource usage and processes
top

ps - display information about running processes
ps aux

kill - terminate a process
kill [PID]

systemctl - control system services and settings
# Start the nginx service
systemctl start nginx
# Check the status of the nginx service
systemctl status nginx
# Stop the nginx service
systemctl stop nginx

service - control system services
service apache2 start

useradd - add a new user to the system
useradd harry

passwd - change the password for a user
passwd harry

userdel - delete a user from the system
userdel harry

su - switch user to become another user
su john

sudo - execute a command as another user or with elevated privileges
sudo

uptime - display system uptime and load average
uptime

df - display disk space usage
df

du - display disk usage by file or directory
du

mount - mount a file system
sudo mount /dev/sdb1 /mnt/usb

umount - unmount a file system
sudo umount /mnt/usb

date - display or set the system date and time
date

whoami - display the current user name
whoami

which - locate a program or command in the system path
ls

finger - displays all the information about user
finger harry

uname - display system information
uname
uname -a

history - display a list of previously executed commands
history

echo - display text or variables to the console
echo 'I need Tshirt from codeswear!'

tee - redirect output to both a file and the console
$ ls | tee file.txt

locate - locate any file on the system
locate file.txt

sort - sort lines of text in a file or input
cat file.txt
banana
orange
apple
sort file.txt
apple
banana
orange

uniq - remove duplicate lines from a file or input
cat file.txt
apple
orange
banana
apple
banana
uniq file.txt
apple
orange
banana


head/tail - display the first/last few lines of a file or input
#display first 10 lines
head file.txt

#display last 10 lines
tail file.txt 

uname -r: kernel version 
uname -o : display os 


ls → List files and directories in the current directory.
ls [directory_name] → List contents of a specific directory.
ls -l → Detailed (long) listing with permissions, owner, size, and date.
ls -a → Show all files, including hidden ones (files starting with .).
ls -lh → Human-readable file sizes (e.g., KB, MB).
ls -lt → Sort by modification time, newest first.
ls -ltr → Sort by modification time in reverse.
ls -i → Show inode numbers of files.
ls -R → List directory contents recursively.
ls -S → Sort by file size, largest first. 



ls -alh → Detailed listing, including hidden files, with human-readable sizes.
ls -R /path/to/dir → Recursively list all files and directories.
ls -lhS → Sort files by size with human-readable output.
ls -ltu → Sort files by access time instead of modification time.
ls -ld  : 1.To check the permissions, ownership, and timestamp of a directory without listing its contents.
          2.Useful when troubleshooting access issues or verifying
