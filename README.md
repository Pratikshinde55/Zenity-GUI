# Zenity

![Configuration of Docker and webser container using Ansible (3)](https://github.com/Pratikshinde55/Zenity-GUI/assets/145910708/3aa299d6-ed4d-40e2-980c-d03259d06768)

## Zenity: 
**Zenity is a powerful command-line utility that allows users to create graphical user interfaces (GUIs) for shell scripts and terminal commands. In this blog post, we'll delve into the various options 
and functionalities offered by Zenity, accompanied by output screenshots for better understanding.**

**Zenity is a handy tool for enhancing the user experience of shell scripts by providing graphical dialogs such as message boxes, input forms, file selection dialogs, progress bars, and more. 
It simplifies interaction with users and adds a visual element to terminal-based applications.**

## How to Install and setup of zenity:

Here i use amazon cloud ubuntu ami and i used putty for ssh connection.(private-key amazon -->> .ppk )

- On putty:

1. In Session -->> Hostname: ubuntu@public_ip_of_instance  -->> select ssh

2. SSH -->>  Auth -->> Credentials -->> private key file for Auth (same key of used for instance)
 
3. SSH -->>  Auth -->>  X11  -->> Enable X11 forwarding 

![Screenshot 2024-04-02 173909](https://github.com/Pratikshinde55/Zenity-GUI/assets/145910708/823dbedc-d7ee-41cc-917a-6c8b3ddfd375)

- Note: 

X11 server need on local window for allow display ,

If don't have then download  "Xming" link for download- [Xming-Download-link](https://sourceforge.net/projects/xming/)  After download install and open onces, it 
can't open just click on open.

- Note:

Also check SSH settings of instance , "/etc/ssh/sshd_config" in this folder allow "X11Forwarding yes". After that just restart sshd by using "systemctl restart sshd" command.

Installation: 

1st need to update use follow command:

     sudo apt-get update

Install command for zenity on ubuntu:

     sudo apt-get install zenity

Check zenity install or not:

     zenity --version


## Magical display commands using Zenity

### Information Dialog:
    
     zenity --info --text="Hello, World!"

![zenity-1](https://github.com/Pratikshinde55/Zenity-GUI/assets/145910708/4ded64e0-54c5-4f63-a368-66b2b1673cf5)

### Warning Dialog:
     
     zenity --warning --text="This is a warning message."

![zenity-2](https://github.com/Pratikshinde55/Zenity-GUI/assets/145910708/7f56b753-83fa-49d0-9487-c0aa6d7a6daa)

### Error Dialog:
     
     zenity --error --text="An error occurred."

![zenity-3](https://github.com/Pratikshinde55/Zenity-GUI/assets/145910708/f27f8224-59d4-4cfd-b294-5147aeaac29a)

### Question Dialog (with Yes/No buttons):
     
     zenity --question --text="Do you want to continue?"

![zenity-4](https://github.com/Pratikshinde55/Zenity-GUI/assets/145910708/bf5038d1-67ed-4c48-a92e-32b3a33142a1)

### Input Dialog (for user input):
     
     zenity --entry --text="Enter your name:"

![zenity-5](https://github.com/Pratikshinde55/Zenity-GUI/assets/145910708/a6f2d6a9-eb55-4867-9b4e-4a9a1fd8fd3e)

### Password Dialog (for password input):
     
     zenity --password --text="Enter your password:"

![zenity-6](https://github.com/Pratikshinde55/Zenity-GUI/assets/145910708/bb67c1e4-1835-46ce-8fed-5ea65f425a26)

### File Selection Dialog (for selecting files):

     zenity --file-selection --title="Select a file:"

![zenity-7](https://github.com/Pratikshinde55/Zenity-GUI/assets/145910708/2bc77b74-9c99-4135-a357-d92c582071d4)

### Calendar Dialog (for selecting a date):

      zenity --calendar --title="Select a date:"

![zenity-8](https://github.com/Pratikshinde55/Zenity-GUI/assets/145910708/5f43cf21-a788-4600-8dc1-a1bd1a562054)

### Progress Dialog (for displaying progress):
      
      zenity --progress --title="Progress" --text="Processing..." --percentage=50

![zenity-9](https://github.com/Pratikshinde55/Zenity-GUI/assets/145910708/15bb824c-818c-41d9-a015-bc0aebf358f2)

### Color Selection Dialog (for selecting a color):
     
     zenity --color-selection --title="Select a color:"

![zenity-10](https://github.com/Pratikshinde55/Zenity-GUI/assets/145910708/a8bd6f6c-0439-4c89-8b2c-c6540df654e2)

### Question Dialog with Custom Buttons:

     zenity --question --text="Do you want to save your changes?" --ok-label="Yes" --cancel-label="No"

![zenity-11](https://github.com/Pratikshinde55/Zenity-GUI/assets/145910708/93ccdbf2-025e-4016-90cc-b8d99a31c8e6)

### Progress Dialog with Auto-Close:

      (sleep 20; echo "100") | zenity --progress --auto-close --text="Processing..."

![zenity-12](https://github.com/Pratikshinde55/Zenity-GUI/assets/145910708/4042897e-87ed-4fd9-88d2-a8e46b7a9b0f)

### Command that displays a "fortune" (random quote) in a dialog window:
here need 1st install fortune-mod on instance. 

       sudo apt install fortune-mod
       
![zenity-13](https://github.com/Pratikshinde55/Zenity-GUI/assets/145910708/cf3a755c-5171-4e21-bb84-39131e34a34f)

![zenity-14](https://github.com/Pratikshinde55/Zenity-GUI/assets/145910708/4d722b86-e1b8-49b7-8321-e81e4801f15a)

Every time new come up:
![zenity-15](https://github.com/Pratikshinde55/Zenity-GUI/assets/145910708/84d34e86-c81e-42a0-ae8b-d2d6977289ae)







