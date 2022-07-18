# INSTALL JAVA JDK ON UBUNTU OPERATIN SYSTEM

## Prerequisites
- A system running Ubuntu 22.04.
- A network connection.
- Access to the command-line/terminal window
- A user account with sudo privileges.

### 1. Check if Java is Installed.
Before installing the Java JDK, check if a Java version is already installed on Windows. Follow the steps below: </p>
Open a terminal and run the following command:

`java --version`

![JavaInstalled](https://res.cloudinary.com/ingenieria/image/upload/v1658123227/it1/ubu1_hlvkbs.jpg)</p>
If it gives you the version of java in the output, then Java is installed on your Ubuntu operating system.

If it gives you this kind of output which is *command java is not found but can be installed whith these commands* then Java is not installed and Ubuntu is suggesting us the versions of Java which we can install.

### 2. Download Java for Ubuntu 22.04
We are interested in installing the oracle Java JDK, so for that Using your preferred web browser, navigate to the [**Oracle Java Downlaoads Page**](https://www.oracle.com/java/technologies/downloads/#jdk17-windows)</p>
![JavaDownload](https://res.cloudinary.com/ingenieria/image/upload/v1658116755/it1/jdkdownload_dakrrg.jpg)</P>
On the Downloads page, click the **x64 debian package** Installer download link under the **Linux** category. At the time of writing this article, Java version 18 is the latest long-term support Java version.</p>
![JavaDownloadx64](https://res.cloudinary.com/ingenieria/image/upload/v1658123227/it1/ubu2_lbjvqm.jpg)</p>
![JavaSave](https://res.cloudinary.com/ingenieria/image/upload/v1658123226/it1/ubu3_lzyl1t.jpg)</p>
Wait for the download to complete.</p>

### 3. Install Java on Ubuntu 22.04
Now the file is downloaded, to start the installation you should use the terminal and type the following command:

`sudo dpkg -i  jdk-18_linux-x64_bin.deb`

And wait for the installation complete.</p>
![Installation](https://res.cloudinary.com/ingenieria/image/upload/v1658123227/it1/ubu4_fpisdd.jpg)</p>

So once that's done we need type the follow two commands:
1. First Command:

    `sudo update-alternatives --install /usr/bin/java java /usr/lib/jvm/jdk-18/bin/java 1`

    ![FCommand](https://res.cloudinary.com/ingenieria/image/upload/v1658123226/it1/ubu5_uh6kgg.jpg)</p>
2. Second Command:
    `sudo update-alternatives --install /usr/bin/javac javac /usr/lib/jvm/jdk-18/bin/javac 1`

    ![SCommand](https://res.cloudinary.com/ingenieria/image/upload/v1658123226/it1/ubu6_fty8li.jpg)</p>


Run the `java --version` command in the terminal to make sure Java installed correctly:</p>
![Verification](https://res.cloudinary.com/ingenieria/image/upload/v1658123226/it1/ubu7_z3lg6b.jpg)</p>
If installed correctly, the command outputs the Java version.</p>

### 4. Set Environmental variables in Java
Some applications require the JAVA_HOME variable. Follow the steps below to create the variable:</p>
1. Type the following command to give you the location for your Java installation folder:

    `sudo update-alternatives --config java`

    ![Folder](https://res.cloudinary.com/ingenieria/image/upload/v1658123226/it1/ubu8_fs45ku.jpg)</p>
2. We are going to add this path as the **JAVA_HOME Environment Variable**. So for that you need to edit a file which is called **etc/profile**, you can use any editor of your choice. 

    To open this file, type the following command in the terminal:

    `sudo gedit /etc/profile`

    ![Editor](https://res.cloudinary.com/ingenieria/image/upload/v1658123226/it1/ubu9_idszkl.jpg)</p>

    At the end of this file you need to just type:

    `JAVA_HOME=/usr/lib/jvm/jdk-18`

    ![TypeCommand](https://res.cloudinary.com/ingenieria/image/upload/v1658123226/it1/ubu11_x9ot1q.jpg)</p>

    Save the changes to the file and close it.
3. To update all the source paths you just need to give this command:

    `source /etc/profile`

    ![Source](https://res.cloudinary.com/ingenieria/image/upload/v1658123225/it1/ubu12_rojogr.jpg)

    Now using this command you can just see the value of your **JAVA_HOME**

    `echo $JAVA_HOME`

    ![Edcho](https://res.cloudinary.com/ingenieria/image/upload/v1658123225/it1/ubu13_iiyrcy.jpg)

[Main Menu](README.md)