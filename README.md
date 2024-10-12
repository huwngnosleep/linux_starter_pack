Here is fast installation scripts and setup for my personal Ubuntu machine
1. Java 23:
  1. Download JDK 23: https://download.oracle.com/java/23/latest/jdk-23_linux-x64_bin.tar.gz
    
    Extract downloaded file and move jdk-23 under /opt
    ```
        sudo mv ~/Downloads/jdk-23_linux-x64_bin/jdk-23 /opt 
    ```
  
2. Maven 
   1. Installation: https://dlcdn.apache.org/maven/maven-3/3.9.9/binaries/apache-maven-3.9.9-bin.tar.gz
   2. Move extracted file under /opt
   3. Setup path

Final. Setup PATH:
    ```
        sudo gedit /etc/profile
    ```
    Paste these:
    ```
        JAVA_HOME=/opt/jdk-23
        MAVEN_HOME=/opt/apache-maven-3.9.9
        PATH=$PATH:$HOME/bin:$JAVA_HOME/bin:$MAVEN_HOME/bin
        export JAVA_HOME
        export JRE_HOME
        export PATH
    ```
    Save the file then log out
