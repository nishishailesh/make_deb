# make_deb
How to make a .deb file for easy installation of a project in debian/ubuntu etc\
There are many help online, but, something covering creation of deb file and dbconf related help in simple language, for newbee are missing\
Requirements:
* Working debian installation
* dekg, dpkg-deb,debconf commands available
* a little bit of shell script idea

It takes inputs
- It makes a shell script in /usr/bin
- It create a .desktop icon for the script
- It create on the fly icon from a small text for use with .desktop file

Basically it does following (for one of my requirements)
 - It create a desktop menu entry
 - When this menu item is selected, it prints a specified file from specified folder
 - The, it cleans folders (deletes all files in folder)
 - This is useful to print same file-name from a browser with minimum user efforts repeatititavely
 
making .deb from here
 - git clone https://github.com/nishishailesh/make_deb
 - go inside make_deb folder
 - dpkg -i ocp.deb
 - answer questions
 - see applications->office
