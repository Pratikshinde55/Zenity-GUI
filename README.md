# Zenity
Exploring Zenity: A Comprehensive Guide with Output Screenshots,Zenity is a powerful command-line utility that allows users to create graphical user interfaces (GUIs) for shell scripts and terminal commands

🌟 Zenity: 
Zenity is a powerful command-line utility that allows users to create graphical user interfaces (GUIs) for shell scripts and terminal commands. In this blog post, we'll delve into the various options 
and functionalities offered by Zenity, accompanied by output screenshots for better understanding.

Zenity is a handy tool for enhancing the user experience of shell scripts by providing graphical dialogs such as message boxes, input forms, file selection dialogs, progress bars, and more. 
It simplifies interaction with users and adds a visual element to terminal-based applications.

⭐How to install and setup:

Here i use amazon cloud ubuntu ami and i used putty for ssh connection.(private-key amazon -->> .ppk )

💥On putty:

1. In Session -->> Hostname: ubuntu@public_ip_of_instance  -->> select ssh

2. SSH -->>  Auth -->> Credentials -->> private key file for Auth (same key of used for instance)
 
3. SSH -->>  Auth -->>  X11  -->> Enable X11 forwarding 

![Screenshot 2024-04-02 173909](https://github.com/Pratikshinde55/Zenity-GUI/assets/145910708/823dbedc-d7ee-41cc-917a-6c8b3ddfd375)


Installation: 

1st need to update use follow command:

     #sudo apt-get update

install command for zenity on ubuntu:

     #sudo apt-get install zenity

Check zenity install or not:

     #zenity --version


