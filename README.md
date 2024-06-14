# findmenu
simple user friendly select menu for the find command

git clone https://github.com/JeremyEngram/findmenu.git /opt;
sudo ln -s /opt/findmenu /usr/local/bin/;
sudo ln -s /usr/local/bin/findmenu ~/Desktop/findmenu;
sudo ln -s /usr/local/bin/findmenu ~/findmenu;



This script provides a user-friendly interface to search for files and directories based on various criteria. It is written in Bash and uses the find command to perform searches.

Features
Find files by extension: Search for files with a specific extension.
Find files matching multiple path/name patterns: Search for files that match multiple path or name patterns.
Find directories matching a given name (case-insensitive): Search for directories with a specific name, case-insensitive.
Find files matching a given pattern, excluding specific paths: Search for files that match a pattern but exclude specific paths.
Find files matching a given size range, limiting the recursive depth: Search for files within a specified size range and limit the search depth.
Run a command for each file: Execute a command for each file found.
Find files modified in the last 7 days: Search for files that were modified in the last 7 days.
Find empty (0 byte) files and delete them: Search for and delete empty files.
Exit: Exit the script.
Usage
Prerequisites
Bash shell
find command
Running the Script
Make the script executable:

bash
Copy code
chmod +x find_files_or_dirs.sh
Run the script:

bash
Copy code
./find_files_or_dirs.sh
Menu Options
Upon running the script, you will be presented with the following menu options:

Find files by extension:

Enter the root path to start the search.
Enter the file extension (e.g., txt, jpg).
Find files matching multiple path/name patterns:

Enter the root path to start the search.
Enter the first path pattern.
Enter the second path pattern.
Enter the file name pattern.
Find directories matching a given name (case-insensitive):

Enter the root path to start the search.
Enter the directory name (case-insensitive).
Find files matching a given pattern, excluding specific paths:

Enter the root path to start the search.
Enter the file name pattern.
Enter the path to exclude.
Find files matching a given size range, limiting the recursive depth:

Enter the root path to start the search.
Enter the minimum size (e.g., 500k).
Enter the maximum size (e.g., 10M).
Run a command for each file:

Enter the root path to start the search.
Enter the command to execute (use {} to access the filename).
Find files modified in the last 7 days:

Enter the root path to start the search.
Find empty (0 byte) files and delete them:

Enter the root path to start the search.
Exit: Exit the script.

Example
To find all .txt files in the /home/user directory:

Run the script:
bash
Copy code
./find_files_or_dirs.sh
Select option 1 from the menu.
Enter /home/user as the root path.
Enter txt as the file extension.
The script will output all .txt files found in the /home/user directory.

License
This project is licensed under the MIT License. See the LICENSE file for details.

Contributing
Feel free to fork this project, submit issues and feature requests, or contribute code. Any help is appreciated!

Replace the example paths and file extensions with the actual paths and extensions you will use in your environment. This README provides a comprehensive guide to using the script effectively.
