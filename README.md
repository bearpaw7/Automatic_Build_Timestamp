Automatic_Build_Timestamp
=========================

How to automatically generate a timestamp upon every build and use the timestamp in code.

Basics
======
You're saving the output of a shell command to a variable in the make environment and then adding that output as a parameter to "-D" compiler option to your CXXFLAGS variable which make uses to form your CXX compiler command.

Background
==========
I needed a way to differentiate build versions on various operating systems, mostly different Linux distributions. Git and SVN versions were great but in between commits, I needed better resolution. I have been using make files for 15 years but never needed anything more than basic compilation until recently.

Caveats
=======
I don't fully understand "=:" as a make function. I think it should save the shell output immediately but I may have seen it run the shell command after every variable reference.
