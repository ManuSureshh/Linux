### Add the new user using the `adduser` command
```
sudo adduser newuser
```

### Set user permissions
- If you want your new user to have sudo privileges, then add it to the sudo group
  ```
  sudo usermod -aG sudo newuser
  ```

### PasswordAuthentication
- If you don't want to use SSH keys but would like to login using password, then
  - Open the SSH configuration file:
    ```
    sudo nano /etc/ssh/sshd_config
    ```
  - Find and modify the following lines:
    ```
    PasswordAuthentication yes
    ChallengeResponseAuthentication no
    ```
- Restart the SSH Service
  ```
  sudo systemctl restart ssh
  ```

- Check the status of SSH service
  ```
  sudo systemctl status ssh
  ```

- Then finally test the Password Authentication

- Adding the new group
  ```
  sudo groupadd group-name
  ```
  
- Adding the user into the group
  ```
  sudo usermod -g group-name user-name
  ```

  
