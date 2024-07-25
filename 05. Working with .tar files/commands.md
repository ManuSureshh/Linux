## Creating a Tar File
### 01. Create a tar archive without compression:
  ```
  sudo tar -cf archive.tar file1.txt file2.txt file3.txt
  ```
  - -c stands for "create"
  - -f specifies the filename of the archive.
![image](https://github.com/user-attachments/assets/9e62e686-052f-4e9a-88a5-f867b8f96ad5)

### 02. Create a gzipped tar archive (common):
  ```
  sudo tar -czf archive.tar.gz file1.txt file2.txt file3.txt
  ```
  - -z enables gzip compression
![image](https://github.com/user-attachments/assets/70b8f200-c0d6-470b-8a01-53f33fccd1ce)

### 03. Create a bzip2-compressed tar archive:
  ```
  sudo tar -cjf archive.tar.bz2 file1.txt file2.txt file3.txt
  ```
  - -j enables bzip2 compression
![image](https://github.com/user-attachments/assets/3790de00-c52d-42e9-be3e-dfba7fc07c7c)

### 04. Create a xz-compressed tar archive:
  ```
  sudo tar -cJf archive.tar.xz file1.txt file2.txt file3.txt
  ```
  - -J enables xz compression
![image](https://github.com/user-attachments/assets/6092b860-3399-42d6-ba45-407c5d571935)

## Extracting a Tar File
### Extract a tar archive:
```
tar -xf archive.tar
```
### Extract a gzipped tar archive:
```
tar -xzf archive.tar.gz
```
### Extract a bzip2-compressed tar archive:
```
tar -xjf archive.tar.bz2
```
### Extract a xz-compressed tar archive:
```
tar -xJf archive.tar.xz
```

![image](https://github.com/user-attachments/assets/813e04e5-f1fc-46fe-b231-2ad56aa4953c)
