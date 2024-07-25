- The path where the software is getting installed can be defined using environment variables.
- Let's change the JAVA version by providing the path of a installed JAVA on linux. 
- Below commands used to check the installed JAVA versions.
  ```
  cd /usr/lib/jvm/
  ls
  ```
  ![image](https://github.com/user-attachments/assets/36a4e3a6-8bd7-4e05-9339-b1e2b7ba3d3f)

- Currently my Linux server is using jdk17.
  ![image](https://github.com/user-attachments/assets/dbf76251-0b7e-4c43-9fac-33aed5305557)

<br>

- Let's open the `.bashrc` and add the JAVA_HOME details in it.
- The `.bashrc` file is a script that is executed whenever a new terminal session is started in a Unix-like operating system. 
```
nano ~/.bashrc
```
- Make sure you added the installed java details into `.bashrc`.
```
# java home
export JAVA_HOME=/usr/lib/jvm/java-11-openjdk-amd64
export PATH=$JAVA_HOME/bin:$PATH
```

![image](https://github.com/user-attachments/assets/fb30ee04-fcca-41c7-a7d5-bb6ed080d595)

- Apply the changes
  ```
  source ~/.bashrc
  ```

- Verify the new JAVA_HOME:
  ```
  echo $JAVA_HOME
  ```

- Also verify the java version.
  ```
  java -version
  ```
  ![image](https://github.com/user-attachments/assets/39145fa4-d60c-4471-a955-173cf27d3dde)

 
  
