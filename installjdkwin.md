# INSTALL JAVA JDK ON WINDOWS OPERATING SYSTEM

## Prerequisites
- A system running Windows 10.
- A network connection.
- Administrador privileges.

[Main Menu](README.md)

### 1. Check if Java is Installed
Before installing the Java JDK, check if a Java version is already installed on Windows. Follow the steps below:
1. Open a command prompt by typing **cmd** in the search bar and **press Enter**.
![CMD](https://res.cloudinary.com/ingenieria/image/upload/v1658116754/it1/cmd_tsu38w.png)
2. Run the following command:

    `java -version`

The command outputs the Java version on your system. If Java isn't installed, the output is a message stating that Java isn't recognized as an internal or external command.
![JavaVerification](https://res.cloudinary.com/ingenieria/image/upload/v1658116755/it1/javaverificacion_gcwjzt.jpg)

### 2. Download Java for Windows 10
Download the latest Java Development Kit installation file for Windows 10 to have the latest features and bug fixes. Follow the steps below:

1. Using your preferred web browser, navigate to the [**Oracle Java Downlaoads Page**](https://www.oracle.com/java/technologies/downloads/#jdk17-windows)</p>
![JavaDownload](https://res.cloudinary.com/ingenieria/image/upload/v1658116755/it1/jdkdownload_dakrrg.jpg)</P>
2. On the Downloads page, click the **x64** Installer download link under the **Windows** category. At the time of writing this article, Java version 18 is the latest long-term support Java version.</p>
![JavaDownloadx64](https://res.cloudinary.com/ingenieria/image/upload/v1658117779/it1/994c9d7f-943d-47b1-b1ba-f8a810fcaf2c_my7mzt.jpg)</p>
![JavaSave](https://res.cloudinary.com/ingenieria/image/upload/v1658117080/it1/41d86ffe-eb63-49c9-b05c-044abb972e9b_cxaamr.jpg)</p>
Wait for the download to complete.</p>

### 3. Install Java on Windows 10
After downloading the installation file, proceed with installing Java on your Windows operating system. Follow the steps below:

1. Run the Download File.<p/>
    Double-click the **downloaded file** to start the installation.<p/>
![OpenDownloadedFile](https://res.cloudinary.com/ingenieria/image/upload/v1658117080/it1/7257a83a-a609-42a4-ac1f-ed589c4e68c9_bmuhf9.jpg)
2. Configure the Installation Wizard.<p/>
    After running the installation file, the installation wizard welcome screen appears.<p/>
    ![Installation](https://res.cloudinary.com/ingenieria/image/upload/v1658117079/it1/20eceb3f-948b-4ef4-af38-34891bfa0658_jdyilh.jpg)</p>
    2.1. Click **Next** to proceed to the next step.<p/>
    ![WelcomeNext](https://res.cloudinary.com/ingenieria/image/upload/v1658117079/it1/040cef68-f845-4359-b1b2-1e7e0a23da69_tqzuq5.jpg)</p>
    2.2. Choose the destination folder for the Java installation files or stick to the default path. Click **Next** to proceed.</p>
    ![DestinatioFolder](https://res.cloudinary.com/ingenieria/image/upload/v1658117079/it1/4e990a84-c1e9-4dcf-ad75-623d26f287c6_ougdrm.jpg)</p>
    ![ChangeDestinationFolder](https://res.cloudinary.com/ingenieria/image/upload/v1658117080/it1/137d7d1b-f65c-4bd4-81b5-e6b93e33805b_nz860s.jpg)</p>
    2.3. Wait for the wizard to finish the installation process until the **Successfully Installed** message appears. Click **Close** to exit the wizard.</p>
    ![WaitInstallation](https://res.cloudinary.com/ingenieria/image/upload/v1658117081/it1/f3e891b6-c75c-4bb3-a1f7-8754d87ec628_ecoxk3.jpg)</p>
    ![SuccessfullyInstalled](https://res.cloudinary.com/ingenieria/image/upload/v1658117080/it1/c48e9e9f-1e87-4844-9a6b-137840480f86_ssqgoh.jpg)</p>

### 4. Set Environmental variables in Java
Set Java environment variables to enable program compiling from any directory. To do so, follow the steps below:

1. Add **Java** to System Variables.</p>
    1.1. Open the Home menu and search for **environment variables**.</p>
    1.2. Select the **Edit the system environment variables** result.</p>
    ![EnvironmentVariables](https://res.cloudinary.com/ingenieria/image/upload/v1658120364/it1/d130cb34-b474-4a46-93ee-fd0b45e90376_y2wfdz.jpg)</p>
    1.3. In the **System Properties** window, under the Advanced tab, click **Environment Variables…**.</p>
    ![SystemProperities](https://res.cloudinary.com/ingenieria/image/upload/v1658120364/it1/ec9ce099-2176-40dc-afe2-52a4ffaa0055_zcyzbu.jpg)</p>
    1.4. Under the System variables category, select the **Path** variable and click **Edit**.</p>
    ![Edit](https://res.cloudinary.com/ingenieria/image/upload/v1658120364/it1/d300358e-3cef-4ec5-bcfc-8341dc154727_r8uxfw.jpg)</p>
    1.5. Click the **New** button and enter the path to the Java bin directory. Click **OK** to save the changes and exit the variable editing window.</p>
    ![NewPath](https://res.cloudinary.com/ingenieria/image/upload/v1658120364/it1/5429a84d-855b-49ab-ba7d-28ac3284d734_y1hjjr.jpg)</p>
    **Note:** The default path is usually *C:\Program Files\Java\jdk-18.0.1\bin*.</p>
2. Add **JAVA_HOME** Variable.</p> 
    Some applications require the JAVA_HOME variable. Follow the steps below to create the variable:</p>
    2.1. In the **Environment Variables** window, under the **System variables category**, click the **New…** button to create a new variable.</p>
    ![NewVariable](https://res.cloudinary.com/ingenieria/image/upload/v1658120364/it1/ffe23e69-4536-47c3-b4b2-405f27c21671_rfffzn.jpg)</p>
    2.2. Name the variable as **JAVA_HOME**. In the variable value field, paste the path to your Java jdk directory and click **OK**. Confirm the changes by clicking **OK** in the **Environment Variables and System** properties windows.</p>
    ![JavaHome](https://res.cloudinary.com/ingenieria/image/upload/v1658120364/it1/34f1c423-5a31-418a-a7ca-55e9f7280c06_v3auxx.jpg)</p>

### 5. Test the Java Installation
Run the `java -version` command in the command prompt to make sure Java installed correctly:</p>
![Test](https://res.cloudinary.com/ingenieria/image/upload/v1658116755/it1/javainstall_qvpsnb.jpg)</p>
If installed correctly, the command outputs the Java version.</p>

[Main Menu](README.md)