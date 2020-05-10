# workshop-javafx-jdbc
Software using javaFX and JDBC

### Prerequisites

* Java 11

* MySQL

### Installing

- **Build JAR file**
    - Open the project in the editor of your choice
    - Right click at project name -> Export -> Java/Runnable JAR file -> Next
    - Select Main class
    - Select destination folder
    - Library handling: 3rd option
    
- **Copy db.properties and JAR file to C:\MyApp**
    - Open the project in the editor of your choice
    - Right click db.properties -> copy
    - Create a folder "MyApp" at C:\
    - Paste the db.properties at this folder
    - Change the user and the password of db.properties according with your MySQL configurations
    - Open the folder where the JAR file was savede, copy the "workshop-javafx-jdbc.jar" and paste at MyApp folder

- **Download JavaFX SDK**
    - Access the link and download the JavaFX SDK (LTS Version), compatible with your Operational System, https://jdk.java.net/archive/
    - Create a folder "jaba-libs" at C:\ and discompact the JavaFX SDK file there
    - Rename the JavaFX-SDK folder for "javafx-sdk"
    - Setup PATH_TO_FX in enviroment variables with the path: C:\java-libs\javafx-sdk\lib
    - Go to JAR file's folder, open "workshop-javafx-jdb_lib", copy "mysql-connector-java-x.x.x.jar" and paste this file at C:\java-libs\javafx-sdk\lib
    
- **Create Windows shortcut**
    - Creat myapp.bat file in MyApp folder and write the script
      ```
      start javaw --module-path %PATH_TO_FX% --add-modules javafx.controls,javafx.fxml -cp programa.jar application.Main
      ```
    - Creat a desktop shortcut with the myapp.bat file path and named as "workshop javafx jdbc"
    
### Running
Double click at "workshop javafx jdbc" shortcut
