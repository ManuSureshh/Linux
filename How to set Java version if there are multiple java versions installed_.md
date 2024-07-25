If you installed multiple Java on a Linux server, then we need to follow the below steps to set one perticular java version.
- For Ubuntu Linux
  ```
  sudo nano .bashrc
  ```
  ```
  sudo vim .bashrc
  ```
  
[or]

  ```
  sudo apt update
  ```
  ```
  sudo apt install gedit
  ```
  ```
  sudo gedit .bashrc
  ```

<br>

Then under
 - `# Set JAVA_HOME`, we need to set the path of a Java version.
 - The path should be the place where the java is installed.
