# ctanzip

This is a bash script written in order to faciliate zipping of packages to upload to CTAN.

Your main package directory should be a git repository. Here's how it works:
- All files not in .gitignore are copied to a directory
- .gitignore is removed from the directory
- The copied directory is zipped
- The original copied directory is removed, leaving only the zip.

## Installation instructions

If you want all users to be able to run the script, place `ctanzip` inside /usr/bin or /usr/local/bin. If you just want the current user to run the script, place `ctanzip` inside ~/bin (assuming your PATH has been set correctly).

## Operating systems

This script is written for Unix-based systems. Thus, if you are on Windows, it is unlikely this script will work (since I don't believe Windows has cp).
