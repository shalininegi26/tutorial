###Logging
The purpose of this tutorial is to demonstrate how to make use of winston, morgan, and file stream rotator to display log information on the console.

###Pre-requisites
You need to install NodeJS on your target host(e.g. Laptop). You can refer to the installation instructions under https://nodejs.org/en/download/.

In case, if you want to clone the entire project then you can install "git" binaries on your target host.

1. Git is pre-installed on MacOS.
2. On Linux host, you can install Git by "sudo yum install git" (for CentOS, Redhat, Fedora) or "sudo apt-get insatll git" (for Ubuntu).
3. You need to create a local copy of this project. For example,

```
git clone https://github.com/quindar/quindar-tutorial.git
 ```
###How to Run the demo
1. After creating a local copy of this project, follow these steps to change the directory

```
cd 06.Logging
cd tutorial6a
```

2. Run the following scripts in order to install NodeJS dependencies and libraries.

```
./buildme.sh

```

3. After successful installation of all dependencies, then type the following in your terminal

```
nodemon server.js

```
You can also use:

```
node server.js
```
In case you face any error regarding log folder not found as it is a hidden file then follow these steps

```
cd tutorial6a
mkdir log
cat > access-20160902.log
```
Then, you can close the file by pressing "control and C". Subsequently, again follow the step 3.

This will let you run HTML page on localhost 3000. On your terminal, you will see the following message appearing on your terminal
"NodeJS Web server listening on port 3000"

Now, open your browser and type "http://localhost:3000" to view our index.html page. This page will give you a description of logging and types of logging.
In order to see our logging information on the console, type "http://localhost:3000/verifyMe" on your browser, and then check on your terminal for logging information about the typed URL.

###Expected Outcome
In this way we can make use of winston, morgan or file stream rotator in our tutorial. For example, now we can make use of logger to display information on the console.
Note that the logger variable is now being used to display information instead of using console.log().



