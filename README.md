**InMemoryFileSystem Class:**

This class represents the in-memory file system. It has the following attributes:

current_directory: Keeps track of the current working directory.
file_system: A dictionary representing the file system structure. Directories are represented by nested dictionaries, and files are represented by strings.
execute_command Method:
This method takes a command as input and executes the corresponding operation. The supported operations include:

mkdir: Create a new directory.
cd: Change the current directory.
ls: List the contents of the current or specified directory.
grep: Search for a pattern in a file (Bonus - not implemented).
cat: Display the contents of a file.
touch: Create a new empty file.
echo: Write text to a file.
mv: Move a file or directory (Bonus - not implemented).
cp: Copy a file or directory (Bonus - not implemented).
rm: Remove a file or directory (Bonus - not implemented).
Directory Manipulation Methods:
mkdir(directory_name): Creates a new directory in the current directory.
cd(path): Changes the current directory based on the provided path.
ls(path): Lists the contents of the specified directory.
File Manipulation Methods:
cat(file_path): Displays the content of the specified file.
touch(file_name): Creates a new empty file in the current directory.
echo(text): Writes text to a file named "output.txt" in the current directory.

**Main Loop:**

The script enters an infinite loop where it continuously prompts the user to enter commands. It calls the execute_command method to process and execute the commands. The loop exits when the user enters "exit."

**Additional Notes:**

Some commands have placeholder comments for bonus functionality (grep, mv, cp, rm). You can implement these as described in the bonus part of the original assignment.
The code is a basic starting point and does not handle many edge cases or errors. In a real implementation, you'd want to add more robust error handling and edge case checks.
You can run this code by executing the script, and then you can interact with the in-memory file system by entering the specified commands during runtime.
