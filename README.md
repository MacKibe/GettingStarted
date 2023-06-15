# GettingStarted

---

Welcome to Mutall Data, here is a documentation on how to install all softwares and tools we use in our daily programming, and how to configure them.  
I will take you through a detailed guideline on how to correctly install all the programs on your system.

Let's start with browsers, we recommend having two or more browsers to carry out your web tests, the browsers are Mozilla Firefox, Google Chrome, Edge, and others..

By default windows users have Microsoft Edge already installed.

### 1. Installing Google Chrome.

- Go to the Google Chrome download page [click here](https://www.google.com/chrome/).
- Click on the "Download Chrome" button.
- Select the correct version of chrome according to your system architecture (32-bit or 64-bit).
- After the download is complete, navigate to the download folder and double-click on the Chrome setup file.
- A user prompt may appear, asking for permission to make changes to your device. Click "Yes" to continue.
- The Chrome installer will now begin. Click "Next" to proceed.
- The installer will ask if you want to "Make Google Chrome the default browser."
- If you want Chrome to be your default browser, click the checkbox next to this option. If not, leave it unchecked.
- Click "Install" to begin the installation process.
- Wait for the installation to complete. It may take a few minutes.
- Once the installation is complete, you will be prompted to "Launch Google Chrome." If you want to start using Chrome right away, click the "Launch" button.  
  If not, you can launch Chrome later by finding it in your Start menu or by searching for it in Windows.

### 2. Installing Mozilla Firefox.

- Go to the Mozilla Firefox download page (https://www.mozilla.org/en-US/firefox/new/)
- Click on the "Download now" button to begin the download.
- Once the download is complete, navigate to the download folder and open the Firefox setup file.
- The Firefox installer will now begin. Click "Next" to proceed.
- The installer will ask if you want to "Customize Firefox." If you want to customize your Firefox installation,  
  click on the "Customize" button to select additional options, such as language and browser data import. If you  
  want to install Firefox with the default settings, click "Next."
- Click "Install" to begin the installation process.
- Wait for the installation to complete. It may take a few minutes.
- Once the installation is complete, you will be prompted to "Launch Firefox." If you want to start using  
  Firefox right away, click the "Launch" button.  
  If not, you can launch Firefox later by finding it in your  
  Start menu or by searching for it in Windows.

Now that we have our browsers set up, let’s start downloading and instaling our programs.

## Visual Studio Code installation Guidelines.

---

Visual Studio Code (VS Code) is a free and open-source code editor, it’s designed for developers working on web and cloud applications and  
supports a wide range of programming languages including but not limited to JavaScript, TypeScript, C#, Python, PHP, Go and more.

The editor includes features such as IntelliSense (code completion), debugging, and Git integration.

It also has a large ecosystem of extensions which can add additional functionality such as additional languages, themes, and debugging tools.

1. Go to the Visual Studio Code website [click here](https://code.visualstudio.com/Download)
2. Click the "Windows" button to get setup for your Windows operating system.
3. Once the download is complete, open the installer file and follow the prompts to install the program.
4. Accept the agreement then click on “Next >”.
5. Broswe the location you would like to install the program.
6. Click “Next >”
7. If you’d like to add additional tasks you can check the checkboxes you would like to add,then click “Next >”
8. Now you can click “Install” and allow the program to install on your system.
9. Once the installation is complete, click “Finish” and Vs Code will launch automatically.

## XAMPP Installation Process.

---

XAMPP is primarily used for web development and local testing of web applications.

It allows developers to test their code on their local machines without the need for a live web server.

1. Go to the Apache Friends website [click here](https://www.apachefriends.org/download.html).
2. Click on the "Download" button for XAMPP.
3. Select the version of XAMPP that you want to install for Windows.
4. Once the download is complete, navigate to the download location and double-click on  
   the installer file to begin the installation process.
5. Click on “Next >” to start installation.
6. Click on “Next >” , you can select components you would like to install on the side menu.
7. Select the folder you will like to install the program, then click on “Next >“.
8. Select the language you will like to install the program, then click on “Next >“.
9. Click on “Next >“.to start the installation.
10. Once the installation is complete, click on the "Finish" button to close the installer.
11. Now open the XAMPP control panel, if you get X on the service section your services have not yet  
    been installed. Double click on the X part to install the various services..
12. When you double click, you will get a prompt to install the service.
13. When the installation is successful you get a green tick symbol to show your service is available.
14. To check if the Apache and MySQL are running, open your web browser and type localhost,  
    you should see the XAMPP start page.
15. Now you can use XAMPP to run web applications locally on your computer and  
    also to test your web pages or websites, on a local server.

### Configuring your apache services to show your projects

1. Open XAMPP Control Panel, On Apache section tap on config, a drop down box will appear
2. Click on Apache (httpd.conf).

3. On the Notepad document, you will edit the DocumentRoot to your directory where your projects are located.
   Note: Have your projects in a different partition from the main computer partitionto reduce problems while using XAMPP.

4. On the “File” tab click on save or you can CTRL + S to save your file, then Close the Notepad.
5. Restart your XAMPP services, then click on “Admin” on the Apache service to open your localhost on the browser.

### Changing Server type from MariaDB to MySQL.

1.  Stop the Apache and MariaDB services in XAMPP Control Panel.
2.  First of all, you will have to download the latest version of the MySQL Community Server from the [official website](https://dev.mysql.com/downloads/mysql/)(Step:1)
3.  Select your Operating system Microsft Windows .(Step:2)
4.  In the Downloads section, select and download the ZIP file “Windows (x86, 64-bit), ZIP Archive”(Step:3)
    You will be redirected to the page shown below, you can continue with the download by clicking on “ No thanks, just start my download” if you dont want to create or login to the Oracle website.
5.  Locate your compress file in your computer, then extract the content
6.  Stop all running instance of Apache or MYSQL
7.  The current working directory is C:\xampp.
8.  Rename the mysql folder in C:\xampp to mariadb
9.  Download the mysql folder from the server into C:\xampp [click here to download the file](!http://206.189.207.206/)
10. You can verify via PHPMyAdmin or you can alternatively use the command line as illustrated below.
11. Now open xampp control panel and start both Apache and MySQL services.
12. Once the services are running, you can open you can run mysql from the command prompt using:

    > cd c:\xampp\mysql\bin

13. Run mysql from the cli with the following command

    > mysql -u root -p

    The output will be:

    > Welcome to the MySQL monitor. Commands end with ; or \g....

14. If you get an 'Mysql Command Not Found' error you need to add mysql to windows environment.

- Navigate to the Windows Start Menu and select This PC.
- Click the Properties tab.
- Now select Advanced System Settings.
- Click the Environment Variables button.
- Single-click the Path system variable, and then click the Edit button.
- Select New to add the correct path for your MySQL folder.
- Retrieve the full path of your MySQL installation. In this example, MySQL is on the C: partition in the Program Files folder.
- Find the bin folder within MySQL and copy the path.
- Paste the full path to the Edit Environment Variable window and click OK to save your changes and exit the screen.
- Restart the cmd interface and enter the initial command once again:

  > mysql -u root -p

## Apache Netbeans 16 Installation Guidelines.

Apache NetBeans is an Integrated Development Environment(IDE) that supports development of all Java application, mobile, web and enterprise applications.  
It includes features such as code completion, debugging, and version control integration.

1. Go to the NetBeans website [https://netbeans.apache.org/download/index.html] and click on the "Download" button.
2. Then select the installer highlighted below for windows user
3. Click on the highlighted link to download the program.
4. Once the download is complete, navigate to the download location and double-click on the installer file to begin the installation process.
5. If you get an error message saying “JDK was not found on this computer” you’ll have to install JDK on your computer, you can continue with JDK installation process below.

### JDK Installation Process.

- Go to the Oracle website [https://www.oracle.com/java/technologies/javase-downloads.html]
- Scroll down to the downloads section and select window option. Then click on the link.
- Once the download is complete, navigate to the download location and double-click on the installer file to begin the installation process.
- Click on “Next >”
- Click on “Next >” if you would like to change the location you can click on “Change”.
- Once the installation is complete, click on the "Finish" button to close the installer.
- Next, set the environment variable on your computer, so that the system knows where the JDK is installed.
  Open the system properties (Right click on My computer -> properties) and click on the advanced system settings.
- Then click on the environment variables.
- Under system variables, scroll down and find the variable named Path, click on edit
- Click on new and paste the path of the JDK bin folder(example: C:\Program Files\Java\jdk1.8.0_251\bin)
- Click on ok and restart your computer for the changes to take effect

6. If you have JDK on your computer, then Click “Next >” to continue with installation, you can click on “Customize” to select packs and runtimes to install.
7. Accept terms in the license agreements and click “Next >”
8. Click “Next >” button if you would like to install the program in the default folder, if not you can select other locations.
9. Click on “Install” to install the program.
10. Once the installation is complete, click on the "Finish" button to launch NetBeans.
11. After the netbeans launch, You may also be prompted to install additional software or plugins, so follow the prompts as necessary.
12. Once you have completed the installation process, you can start using NetBeans to develop your Java applications.

### Configuring your Debugger.

1. You will check if the debugger is installed on your system.

- Create a file named info.php
- Open the file on the browser.
- Copy the all the content in the result website
- Paste the content in the textfield
- Then click on “analyse my phpIno() output”
- You will be redirected to (https://xdebug.org/wizard)
- Download **php_xdebug-3.2.0-8.1-vs16-x86_64.dll**
- Move the downloaded file to C:\xampp\php\ext, and rename it to php_xdebug.dll
- Update C:\xampp\php\php.ini and add the following lines:

  > zend_extension = xdebug
  >
  > xdebug.start_upon_error = yes
  >
  > xdebug.client_port = 9000
  >
  > xdebug.mode = debug
  >
  > xdebug.client_host = localhost

- Restart the Apache Webserver

2. Open your info.php on browser to check if the Xdebug is installed correctly,

- Search for xdebug,
- If you get it then you have successfully installed it.

### Upload projects to the server using Netbeans.

1. Open NetBeans on your computer.
2. Create a new project or open an existing one.
3. Right-click on your project in the "Projects" tab and select "Properties".
4. In the "Properties" window, select the "Run" category.
5. In the "Run As" dropdown menu, select "Remote Web Site".
6. In the "Remote Connection" section, click on the "Manage..." button.
7. In the "Manage Remote Connection" window, click on the "New..." button.
8. Enter the details of the server you want to connect to, including the host name or IP address, the port number, and the type of protocol you want to use (FTP or SFTP).
9. Enter your login credentials for the server, including your username and password.
10. Click "Next" to test the connection. If the connection is successful, click "Finish" to save the settings.
11. In the "Properties" window, click "OK" to save the changes.
12. Right-click on your “Source code” in your project in the "Projects" tab and select "Upload Files".
13. In the "Upload Files" window, select the files or folders you want to upload.
14. Click "Upload" to start the upload process.
15. Once the upload is complete, you will receive some successful messages in the terminal of Netbeans and you can also confirm in the server if your foles have been uploaded.

## Installing Node js.

1. Go to the Node.js website at (https://nodejs.org)
2. Click on the "Download" button to download the Node.js installer for your operating system. Node.js is available for Windows, macOS, and Linux.
3. Run the Node.js installer that you downloaded.
4. Follow the instructions in the installer to complete the installation process. Read and accept the Terms and Conditions
5. By default, Node.js will be installed in the "Program Files" or "Program Files (x86)" folder on Windows, or the "/usr/local/bin" folder on macOS and Linux.
6. Once the installation is complete, open a terminal or command prompt window.
7. Type **node -v** and press Enter to check that Node.js has been installed correctly. You should see the version number of Node.js displayed in the terminal.
8. Type **npm -v** and press Enter to check that the Node Package Manager (npm) has been installed correctly. You should see the version number of npm displayed in the terminal.

## Installing Filezilla.

FileZilla is a free and open-source FTP client and FTP server software. It supports various protocols such as FTP, SFTP, and FTPS.  
The client features a user-friendly interface, drag and drop support, and the ability to resume interrupted transfers.  
The server version allows for easy setup and management of FTP connections. FileZilla is widely used for transferring files between a local computer and a remote server.

1. Go to the FileZilla website (https://filezilla-project.org/) and click on the "Download" button.
2. Select the version of FileZilla that is appropriate for your system (32-bit or 64-bit).
3. Once the download is complete, navigate to the download folder and double-click on the FileZilla setup file.
4. A User Account Control prompt may appear, asking for permission to make changes to your device. Click "Yes" to continue.
5. The installer will ask you to agree the license agreement, Click on “Agree”
6. You might be requested to install brave, if you would like to install brave browser select “Accept” or select “Decline” to continue with Filezilla installation.
7. You select users who will get access to Filezilla program, you can leave it on default to allow all users to have access. Click "Next" to proceed
8. The installer will ask if you want to "Create a desktop icon." If you want to create a desktop icon, click the checkbox next to this option. If not, leave it unchecked.
9. The installer will ask if you want to "Create a quick launch icon." If you want to create a quick launch icon, click the checkbox next to this option. If not, leave it unchecked. Click "Next" to proceed.
10. Wait for the installation to complete. It may take a few minutes.
11. Once the installation is complete, you will be prompted to "Launch FileZilla." If you want to start using FileZilla right away, click the "Launch" button. If not, you can launch FileZilla later by finding it in your Start menu or by searching for it in Windows.
12. Once the FileZilla is launched, you will be prompted to create a new connection. Enter the server details and click on "Connect" to connect to the FTP server.

### How to upload projects to the server using filezilla.

1. Open up your Filezilla program,enter the details of the server you want to connect to. This includes the host name, the username the port number, and password which are provided below.

#### Server Details for Mutall.

> Host name : sftp://206.189.207.206
>
> Username : Mutall
>
> The password we will provided to you.
>
> Port: 22

2. Once you have entered all the required details, click on the "Connect" button to establish a connection to the server.
3. After you have established a connection, you will see two panes in the FileZilla window. The left pane shows the files and folders on your local computer, while the right pane shows the files and folders on the remote server.
4. To upload files to the server, simply select the files or folders you want to upload in the left pane and then drag them to the desired location in the right pane. You can also use the upload button on the toolbar, which looks like an arrow pointing upwards.
5. Once you have uploaded the files, you can check that they have been successfully uploaded by refreshing the right pane. The newly uploaded files should now appear in the folder you uploaded them to.
6. You are also required to have git in your system.

## Installing Git.

Git is a version control system (VCS) that is used for tracking changes in computer files and coordinating work on those files among multiple people.  
Git allows developers to work on the same codebase simultaneously by keeping track of changes made to the files and allowing different versions to be merged together seamlessly.  
This makes it easy for teams of developers to collaborate on the same project, and also makes it easy to roll back to previous versions of the code if something goes wrong.  
Git also provides a powerful set of tools for managing and reviewing changes, such as branching, merging, and diffing, which help developers keep track of their codebase and collaborate more effectively.

1. To install Git, you will first need to download the installer for your operating system from the official Git website (https://git-scm.com/downloads)
2. Select the correct version of according to your system architecture (32-bit or 64-bit).
3. Once the installer has been downloaded, run it and follow the prompts to complete the installation.
4. Click on “next”
5. If you would like to change the destination, select bowse and change location otherwise you can, Click on “Next” to continue with the default one.
6. Select components you would like to be installed, then click on “Next”.
7. You can select “Dont create a Start Menu Folder” if you dont want to have a shortcut created on the desktop, then click on “Next”.
8. Select editor you would like to be using, then click on “Next”.
9. Select the your initial branch name, to use the default branch name you can select “Let git decide” option. Or select “Override the default branch name for new repositories” and add your custom name.
10. Click on “Next” to continue with the default path environment.
11. Click on “Next” to use the handled OpenSSH.
12. Select library to use for HTTPs connection, then Click on “Next”
13. Select how you would like git to treat the endings of text files, then click “Next”
14. Select which terminal emulator you would like git bash to be using, then click “Next”.
15. Select the default behaviour of git pull, then click on “Next”
16. Choose creditian helper, then click on “Next”.
17. Check which extra features you would like to enable, then click on “Next”
18. Click on “Install” to finish installation, it might take some time to install, then click on “Finish” to close the installer dialog page.
19. To verify that Git has been installed correctly, you can open a terminal or command prompt and type "git --version". This should return the version number of Git that you have installed.
20. To start using git, you will have to set up your username and email using the command:

    > git config --global user.name "Your Name"
    >
    > git config --global user.email "youremail@example.com"

21. You can check the config by using:

    > git config --list

22. You can now use git for version control in your local machine.

### How to install it on your machine:

- One last item you need to have in your system is the Acer projector software for presenting your work.

1. Open the acer projector website,make sure your connected to the mutual network and the projector is also on the same network (http://192.168.100.217/cgi-bin/welcome.cgi?lang=en)
2. Download the acer projector software, select Windows OS for windows users.
3. Once the setup is downloaded, double click on it on the setup.
4. When the acer projection applications click on the play button to connect to the projector.

## ANDROID STUDIO

---

1. Download Android Studio: Go to the official website of Android Studio (https://developer.android.com/studio) and click on the "Download Android Studio" button. You can choose the latest version based on your operating system.
2. Run the Android Studio setup: Once the download is complete, run the Android Studio setup file. You may be prompted with a security warning, click "Yes" or "Allow" to proceed.
3. Choose components: In the next window, you can choose which components to install. Generally, the default components are sufficient for most users, so you can click on "Next" to proceed.
4. Choose installation location: You can choose the installation location for Android Studio on your computer. If you want to use the default location, just click "Next" to proceed.
5. Select Start Menu Folder: You can choose whether you want to create a shortcut for Android Studio in the Start menu folder. Click "Install" to proceed.
6. Wait for installation: The installation process may take a few minutes to complete. Wait for the progress bar to finish.
7. Launch Android Studio: Once the installation is complete, click on the "Finish" button to launch Android Studio.
8. Configure Android Studio: Android Studio may prompt you to configure some settings, such as setting up a new project or importing an existing one.
9. After the Android Studio installation wizard has completed, you will need to follow these steps to set up Android Studio:
10. Accept the Terms and Conditions: When you launch Android Studio for the first time, you will be prompted to accept the terms and conditions of the software. Read the terms and conditions carefully and click on the "I Agree" button.
11. Choose a theme: You can choose a theme for Android Studio based on your preference. You can select "Dark", "Light" or "Custom". You can also skip this step by clicking on the "Skip" button.
12. Install Android SDK: After accepting the terms and conditions, you will be prompted to install the Android SDK. The SDK is required to develop Android applications. You can either choose to install the recommended SDK or choose a custom SDK location.
13. Set up the Android Virtual Device (AVD) Manager: The Android Virtual Device Manager is used to create and manage virtual devices that emulate different Android devices. You can create an AVD by clicking on the "AVD Manager" button and then clicking on the "Create Device" button.
14. Create a new project: Once you have set up the SDK and AVD, you can create a new Android project. Click on the "Create New Project" button and follow the instructions to create a new Android project.

## For Linux Users.

---

1. Run the updater command

   > sudo apt update

2. Enter your System root password
3. Then run the upgrade command

   > sudo apt upgrade

4. Press Y to continue
5. Then run the autoremove command

   > sudo apt autoremove

6. Press Y to continue

Step -1: **Install Apache Web Server on ubuntu.**

1. Install apache2 with the following command.

   > sudo apt install apache2 -y

2. Whether Apache web server is successfully installed or not goto browser and type anyone form following in address bar

   > http://localhost/
   >
   > http://127.0.0.1/
   >
   > http://your_machine_ip_address/

3. Enable firewall settings by following commands :

   > sudo ufw status
   >
   > sudo ufw enable
   >
   > sudo ufw app list
   >
   > sudo ufw allow in "Apache Full"

Step - 2: **Install mysql-server on ubuntu.**

1. Install mysql with the following command.

   > sudo apt install mysql-server

2. Then press Y to continue
3. Login mysql with root user without password with sudo

   > sudo mysql

4. Create a database in the mysql kernel.

   > create database db_name;
   >
   > use db_name;
   >
   > select database();
   >
   > exit
   > Step - 3: Install php and its required libraries:

5. Install mysql with the following command.

   > sudo apt install php php-mysql libapache2-mod-php

6. Press Y to continue
7. Check if php is installed successfully with the following command.

   > php -v

8. Create one sample php file in Apache Web server root directory

   > Go to the root directory.
   >
   > > cd /var/www/html
   > > Create a file.php
   >
   > > sudo gedit file_name.php
   > > Go to browser and run
   >
   > > http://localhost/file_name.php

9. Change permission for apache root directory.

   > sudo chown -R $USER:$USER /var/www/html

10. Create a php file without sudo through terminal using gedit or any other text editor.

    > gedit file_name.php

11. Goto browser and run

    > http://localhost/file_name.php

Step - 4: **Install PHPMyAdmin.**

1. Run the updater command

   > sudo apt update

2. Enter your System root password
3. Then run the upgrade command

   > sudo apt upgrade

4. Press Y to continue
5. Install mysql with the following command.

   > sudo apt install phpmyadmin

6. Press Y to continue
7. Select Apache2 by pressing space and then press tab and OK
8. Press Yes and set password for dummy user phpMyAdmin
9. Restart apache2.

   > sudo systemctl restart apache2

10. Check whether phpMyAdmin is successfully installed or not, goto browser and type

    > (http://localhost/phpmyadmin)

11. Default user name is “phpMyAdmin” and enter your password which added during the configuration.
12. Run update

    > sudo apt update

13. Set root password and create a new database user with full privileges

    > sudo mysql
    >
    > SELECT user,authentication_string,plugin,host FROM mysql.user;
    >
    > ALTER USER ‘root’@‘localhost’ IDENTIFIED WITH caching_sha2_password BY ‘password’;
    >
    > SELECT user,authentication_string,plugin,host FROM mysql.user;
    >
    > exit

14. Run the following to login with password

    > sudo mysql -p

15. Enter your password

    > CREATE USER ‘new_user’@‘localhost’ IDENTIFIED WITH caching_sha2_password BY ‘password’;
    >
    > GRANT ALL PRIVILEGES ON . TO ‘new_user’@‘localhost’ WITH GRANT OPTION;
    >
    > exit

16. Once again restart apache and mysqql with the following command

    > sudo systemctl restart apache2 && sudo systemctl restart mysql

17. Goto web browser and type

    > (http://localhost/phpmyadmin)

18. Enter new username and password. Now you can create databases, tables and execute some queries through the phpmyadmin site.

Step - 4: **Install Git..**

1. It's a good idea to make sure you're running the latest version. To do so, Navigate to your command prompt shell and run the following command to make sure everything is up-to-date:

   > sudo apt-get update

2. To install Git, run the following command

   > sudo apt-get install git-all

3. Once the command output has completed, you can verify the installation by typing:

   > git version

Step - 5 : **Installing FileZilla client.**

1. To install FileZilla client from the command line, use the following commands.

   > sudo apt-get update
   > sudo apt-get install filezilla

2. The following command prints the version of the installed FileZilla client.

   > filezilla --version
