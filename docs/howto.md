# How-to guide

Here we gather a collection of how-to notes to help users self-managing their virtual machines.

# Remote desktop connection

When a project requires access to a remote desktop we preconfigure virtual machines with
[Apache Guacamole](https://guacamole.apache.org).

## How to change your password in Guacamole

Go to the menu on the top-right and click on **Settings**:

![](images/guac-menu-user.png)

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
* Connections/SSH

![](images/guac-add-user-3.png)
