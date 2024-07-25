## 1. Viewing Processes

- ps: This will display information about active processes.
  ```
  ps aux
  ```
  Example: -
  ```
  ps aux | grep nginx
  ```

- top: Real-time display of system summary information and list of processes.
  ```
  top
  ```

- htop: Interactive process viewer (similar to top but more user-friendly).
  ```
  htop
  ```

- pgrep: Search for processes based on name and other attributes.
  ```
  pgrep sshd
  ```

- pidof: Find the process ID of a running program.
  ```
  pidof httpd
  ```

- pstree: Display a tree of processes.
  ```
  pstree
  ```

## 2. Managing Processes

- kill : Send a signal to a process, typically to terminate it.
  ```kill 1234
     kill -9 1234  # Forcefully terminates the process
  ```
  
- pkill : Send a signal to processes based on name and other attributes.
  ```
  pkill sshd
  ```
  
- killall : Kill processes by name.
  ```
  killall httpd
  ```
  
- renice : Change the priority of an already running process.
  ```
  renice 10 1234
  ```
  
- nice : Run a command with a modified scheduling priority.
  ```
  nice -n 10 command_name
  ```

## 3. Job control
- bg: Resume a suspended job in the background.
  ```
  bg %1
  ```
  
- fg: Bring a background job to the foreground.
  ```
  fg %1
  ```
  
- jobs: List active jobs.
  ```
  jobs
  ```
  
- disown: Remove jobs from the job table.
  ```
  disown %1
  ```
  
## 4. Monitoring and Debugging
- strace: Trace system calls and signals.
  ```
  strace ls
  ```
  
- lsof: List open files by processes.
  ```
  lsof
  lsof -i :80  # List processes using port 80
  ```
  
- vmstat: Report virtual memory statistics.
  ```
  vmstat
  ```
  
- iostat: Report CPU and I/O statistics.
  ```
  iostat
  ```
  
- sar: Collect, report, or save system activity information.
  ```
  sar -u 1 3  # CPU usage every 1 second, 3 times
  ```

## 5. Resource Limits
- ulimit: Set or get limitations on the resources available to the shell and processes started by it.
  ```
  ulimit -a
  ```

## 6. Other Utilities
- uptime: Tell how long the system has been running.
  ```
  uptime
  ```
  
- watch: Execute a program periodically, showing output fullscreen.
  ```
  watch df -h
  ```
  
- nohup: Run a command immune to hangups, with output to a non-tty.
  ```
  nohup long_running_command &
  ```
  
- at: Schedule a command to run at a particular time.
  ```
  echo "backup.sh" | at 02:00
  ```
  
- cron: Schedule regular background jobs.
  ```
  crontab -e
  ```



  
