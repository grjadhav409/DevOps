Linux Short Notes

For DevOps Engineers

History of Linux

	•	Linux originated from Unix and is a free, open-source operating system developed by Linus Torvalds in September 1991.
	•	Linus Torvalds was a student at the University of Helsinki, Finland, when he posted the Linux 0.01 code on the Minix newsgroup. The first official version, Linux 0.02, was released on October 5, 1991.
	•	Linux has grown to power 90% of the top 500 supercomputers globally.

Linux File System Hierarchy

	•	Everything is a file in Linux, and files are stored in a directory with a tree structure called the File System Hierarchy (FSH).
	•	The root directory is represented by / (forward slash), and every directory starts from it.

Important Directories:

	•	/root: Home directory for the root user (superuser).
	•	/bin: Contains user binaries, common Linux commands used by all system users.
	•	/sbin: System binaries used for system maintenance, typically by system administrators (e.g., iptables, reboot, ifconfig).
	•	/dev: Contains hardware device files (e.g., terminal devices, USB devices).
	•	/var: Variable data files, such as logs and temporary files.
	•	/mnt: Used to mount a file system temporarily.
	•	/media: Contains removable media devices.
	•	/usr: Applications and files used by users.
	•	/etc: Configuration files of the server, startup, and shutdown program scripts.
	•	/boot: Boot loader files and kernels.
	•	/opt: Optional software from third-party vendors.
	•	/home: Home directory for secondary users.
	•	/tmp: Temporary files, deleted upon reboot.

Basic Linux Commands

	•	pwd: Shows the present working directory.
	•	ls: Lists files and directories in the current directory.
	•	uname: Displays the OS name and version.
	•	cd: Changes the directory.
	•	clear: Clears the screen.
	•	whoami: Displays the currently logged-in user.
	•	history: Shows a list of previously used commands.
	•	date: Shows the current date and time.

File Management

	•	Touch command: Creates empty files.
	•	cp command: Copies files and directories.
	•	Options: -r (recursive), -v (verbose), -f (force).
	•	mv command: Moves or renames files and directories.
	•	rm command: Removes files or directories.

User Management

	•	Commands for creating, deleting, and managing user accounts.
	•	Group management: Adding or removing users from groups and managing group permissions.

Linux File System Permissions

	•	Basic Permissions: r (read), w (write), x (execute).
	•	File Ownership: Owner (u), group (g), others (o).
	•	ACL (Access Control List): Allows for flexible permission control for specific users or groups without adding them to the primary group.

Regular Expressions and GREP

	•	GREP: A command to search for patterns in files using regular expressions.
	•	Useful for searching strings across multiple files, matching patterns, and inverting matches.

Find Command

	•	Used to search files and directories based on different criteria like permissions, users, groups, file size, and more.

Word Count (WC) Command

	•	wc command: Counts the number of lines and words in a file.

Head and Tail Commands

	•	head: Displays the top lines of a file.
	•	tail: Displays the bottom lines of a file.

Archiving Files

	•	tar command: Used for archiving and compressing files.
	•	Common options: -c (create), -x (extract), -v (verbose), -z (gzip compression), -j (bzip2 compression), -J (xz compression).

Job Automation

	•	at command: Executes a job one time.
	•	crontab: Executes recurring jobs at scheduled intervals.

Sudo Command

	•	sudo: Allows permitted users to execute commands as another user, including the superuser (root).
	•	Configuration is handled via the /etc/sudoers file.
	•	Sudo without a password can be configured for users or groups.

Networking in Linux

	•	nmcli command: Used to manage networking, show active connections, and configure IP addresses.
	•	nmtui: Text-based user interface for configuring network settings.
