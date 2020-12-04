# How-to guide

Here we gather a collection of how-to notes to help users self-managing their virtual machines.

# User management

Initially there is only one preconfigured user account on the virtual machine, the **spsrc** user,
with privileges to create new accounts for your collaborators.

## Change your default password

Run the following command on a terminal and follow instructions:
```
passwd
```

## Create a user account

Open a terminal and run the following commands:
```
# Generate a new password hash:
openssl passwd

# Create a new account:
sudo useradd --password "<output-from-previous-command>" --gid spsrc-group --create-home --shell /bin/bash <collaborator>
```
For example:
```
# Create a new account:
sudo useradd --password "<output-from-previous-command>" --gid spsrc-group --create-home --shell /bin/bash john
```

## Delete a user account

Here are the steps:
```
sudo userdel <collaborator> --remove
```
For example:
```
sudo userdel john --remove
```

# Software installation

All users are granted with **sudo** privileges to use the operating system package manager
(i.e. **apt-get** in Ubuntu, and **yum/dnf** in Centos7/8) to install packages via the official
repositories. 

# SSH access

SSH access into virtual machines is only allowed via public-key authentication.
Please send your public key to ska-itsupport 'at' iaa.csic.es and we will configure your SSH access.

# Remote desktop: Guacamole

When a project requires access to a remote desktop we preconfigure virtual machines with
[Apache Guacamole](https://guacamole.apache.org).

## Working with the clipboard in Guacamole

Using the clipboard in Guacamole is not intuitive. If you are planning to use the clipboard a lot,
and the information you are going to work with is available online (i.e. via a web browser), we then
recommend you to open firefox to copy/paste as usual inside the virtual machine.

If, on the other hand, you need to copy/paste between your workstation and the virtual machine, then
you will have to use the Guacamole menu. On the tab where you have Guacamole working, press **Ctrl+Alt+Shift** 
and the menu appears on the left:

![](images/guac-clipboard.png)

You will see the Guacamole clipboard that will be used as an intermediate buffer between your workstation
and the virtual machine:

* Copy/paste from your workstation to the virtual machine: 1) first copy the text into the clipboard
as usual in your workstation; 2) open the Guacamole menu with **Ctrl+Alt+Shift** and paste your text
into the Guacamole clipboard; 3) the text is now available inside the virtual machine clipboard and
you can paste it as expected with **Ctrl+V**

* Copy/paste from the virtual machine to your workstation: 1) use **Ctrl+C** inside the virtual machine
to copy text as usual; 2) open the Guacamole menu with **Ctrl+Alt+Shift** and copied text automatically
appears in the Guacamole clipboard; 3) you can now copy from there into your workstation's clipboard.

## How to change your password in Guacamole

Press **Ctrl+Alt+Shift** to open the Guacamole menu, first click on your username (**spsrc** on the
example image) and then on **Settings**:

![](images/guac-change-pass.png)

Then go to **Preferences** and follow instructions to change your password:

![](images/guac-change-pwd.png)

## How to add a new user in Guacamole

Go to the menu on the top-right and click on **Settings**:

![](images/guac-menu-user.png)

Then go to **Users** and click on **New User**:

![](images/guac-add-user-1.png)

Enter a username and password for the new user:

![](images/guac-add-user-2.png)

Scroll down and check the following and click on **Save**:

* Permissions/Change own password
* Connections/RDP

![](images/guac-add-user-3.png)
