Here is fast installation scripts and setup for my personal Ubuntu machine
1. Install needed technologies
   1. Java 23:
      1. Download JDK 23: https://download.oracle.com/java/23/latest/jdk-23_linux-x64_bin.tar.gz
        Extract downloaded file and move jdk-23 under /opt
        ```
            sudo mv ~/Downloads/jdk-23_linux-x64_bin/jdk-23 /opt 
        ```
      2. Setup JAVA_HOME AND PATH:
        ```
            sudo gedit /etc/profile
        ```
        Paste these:
        ```
            JAVA_HOME=/usr/lib/jvm/jdk1.7.0
            PATH=$PATH:$HOME/bin:$JAVA_HOME/bin
            export JAVA_HOME
            export JRE_HOME
            export PATH
        ```
        Save the file then log out

