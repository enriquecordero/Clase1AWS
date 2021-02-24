## Instalar Java
1. Vamos a instalar el JDK de OPENJDK  http://openjdk.java.net/install/
   ```sh
   yum install java-1.8*
      ```

1. Confirm Java Version and set the java home
   ```sh
   java -version
   find /usr/lib/jvm/java-1.8* | head -n 3
   JAVA_HOME=/usr/lib/jvm/java-1.8.0-openjdk-<Java version which seen in the above output>
   export JAVA_HOME
   PATH=$PATH:$JAVA_HOME
    # To set it permanently update your .bash_profile
   vi ~/.bash_profile

   
   ```
   _The output should be something like this,_
    ```sh
   [root@~]# java -version
   openjdk version "1.8.0_151"
   OpenJDK Runtime Environment (build 1.8.0_151-b12)
   OpenJDK 64-Bit Server VM (build 25.151-b12, mixed mode)