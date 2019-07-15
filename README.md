# Lambda School Web API: Java Course 
## Software installations for Week 2 

<details><summary>For All Operating Systems</summary>
<p>

### Nothing to install that is NOT operating system specific. See your OS link for installation instructions

</p>
</details>


<details><summary>For Windows 10 Operating System</summary>
<p>

### Install PostgreSQL on a Windows 10 based computer

[![Video to Install PostgreSQL](http://img.youtube.com/vi/y1DV86i9vDY/0.jpg)](http://www.youtube.com/watch?v=y1DV86i9vDY)

* Download and install the software from [https://www.enterprisedb.com/downloads/postgres-postgresql-downloads](https://www.enterprisedb.com/downloads/postgres-postgresql-downloads)
* Install all the available software from the download. At the end, you do not need to launch Stack Builder at this time.
* You must restart your machine after this install.

---
### Install Postman on a Windows 10 based computer

[![Video to Install Postman](http://img.youtube.com/vi/q-cw1IVvgzQ/0.jpg)](http://www.youtube.com/watch?v=q-cw1IVvgzQ)

Download and install the software from [https://www.getpostman.com/](https://www.getpostman.com/)

---
</p>
</details>


<details><summary>For Mac OS</summary>
<p>

### Install PostgreSQL on a Mac OS Computer

[![Video to Install PostgreSQL](http://img.youtube.com/vi/JU7rIkXyQYs/0.jpg)](http://www.youtube.com/watch?v=JU7rIkXyQYs)

* Download and install the software from [https://www.enterprisedb.com/downloads/postgres-postgresql-downloads](https://www.enterprisedb.com/downloads/postgres-postgresql-downloads)
* Install all the available software from the download. At the end, you do not need to launch Stack Builder at this time.
* You must restart your machine after this install.

NOTE:

If you run into issues, try entering the following command in a terminal window. Then try to reinstall!  
```sudo spctl --master-disable```

---
### Install Postman on a Mac OS Computer

[![Video to Install Postman](http://img.youtube.com/vi/PSrRNnZgLXI/0.jpg)](http://www.youtube.com/watch?v=PSrRNnZgLXI)

Surf to the website [https://www.getpostman.com/](https://www.getpostman.com/) and install the software</p>

---
### Set Environment Variables for a MAC OS Computer

[![Video to Environment Variables](http://img.youtube.com/vi/XCDOh4GPNZk/0.jpg)](http://www.youtube.com/watch?v=XCDOh4GPNZk)

Environment variables are needed for
* Class
* Build Week
* Labs
* Industry

Why set environment variables 
* prevent adding passwords and such to github
* restrict knowledge of the passwords and such to the executing machine

To show all environment variables 
```
printenv
```

To show a specific environment variable
```
echo $PATH
```

To set up environment variables permanently
```
Go to home directory
cd
nano .bash_profile
```

move to the end of the file. Add a new line and enter the following:
```
export MYDBPASSWORD=password
export MYDBUSER=postgres
export LAMBDACLIENT=lambda-client
export LAMBDASECRET=lambda-secret
```
Restart the computer!

---
</details>


<details><summary>For Linux specifically Ubuntu 18</summary>
<p>
  
### Install PostgreSQL on a Linux Computer

[![Video to Install PostgreSQL](http://img.youtube.com/vi/XuiaSJAVtNo/0.jpg)](http://www.youtube.com/watch?v=XuiaSJAVtNo)

To install PostgreSQL, enter the following from a terminal prompt

* sudo nano /etc/apt/sources.list.d/pgdg.list
** enter the following line   
```deb http://apt.postgresql.org/pub/repos/apt/ bionic-pgdg main```   
** exit nano
* wget --quiet -O - https://www.postgresql.org/media/keys/ACCC4CF8.asc | sudo apt-key add -
* sudo apt update
* sudo apt install postgresql-11
* sudo apt install postgresql-client-11
* sudo apt install pgadmin4

* sudo -u postgres psql
* ALTER USER postgres PASSWORD 'password';
* \q

* run pgadmin4 from APPs   
Create a link to the server</p>

---
### Install Postman on a Linux Computer

[![Video to Install Postman](http://img.youtube.com/vi/4yMn6h0_MGI/0.jpg)](http://www.youtube.com/watch?v=4yMn6h0_MGI)

To install Postman, from a terminal prompt enter
* sudo apt update
* sudo apt install libgconf-2-4

Surf to the website [https://getpostman.com](https://getpostman.com)
* Download the software in a compressed file
* Extract the file to some location, like your home directory

Create a Desktop entry for Postman. It should be saved as   
```~/.local/share/applications/Postman.desktop```   
and contain the following

```
[Desktop Entry]
Encoding=UTF-8
Name=Postman
Exec=/home/<your account>/Postman/app/Postman %U
Icon=/home/<your account>/Postman/app/resources/app/assets/icon.png
Terminal=false
Type=Application
Categories=Development;
```

### Set Environment Variables for a Linux Computer

[![Video to Environment Variables](http://img.youtube.com/vi/IyGr-cJePIk/0.jpg)](http://www.youtube.com/watch?v=IyGr-cJePIk)

Environment variables are needed for
* Class
* Build Week
* Labs
* Industry

Why set environment variables 
* prevent adding passwords and such to github
* restrict knowledge of the passwords and such to the executing machine

To show all environment variables 
```
printenv
```

To show a specific environment variable
```
echo $PATH
```

To set up environment variables permanently
```
Go to home directory
cd
nano .bashrc
```

move to the end of the file. Add a new line and enter the following:
```
export MYDBPASSWORD=password
export MYDBUSER=postgres
export LAMBDACLIENT=lambda-client
export LAMBDASECRET=lambda-secret
```
Restart the computer!

---
---
</p>
</details>
