# Linux Find Command

Using find command to search for file or directory

<!-- ----------------------------------------------- -->
## Find files based on filename

```
find [directory path] -type f -name [filename]
```

Example: find /home/Andy -type f -name sales.txt <br><br>

<!-- ----------------------------------------------- -->
## Find Directory based on directory name

```
find [directory path] -type d -name [filename]
```

Example: find /home/Andy -type d -name pictures <br><br>

<!-- ----------------------------------------------- -->
## Find files based on size

```
find [directory path] -type f -size [size]
```

Example: find /home/Andy -type f -size 10c <br>
*(c for bytes, k for kilobytes, M megabytes, G for gigabytes)* <br><br>

<!-- ----------------------------------------------- -->
## Find files based on username

```
find [directory path] -type f -user [username]
```

Example: find /etc/server -type f -user john <br><br>

<!-- ----------------------------------------------- -->
## Find files based on group name

```
find [directory path] -type f -group [group name]
```

Example: find /etc/server -type f -group teamstar <br><br>

<!-- ----------------------------------------------- -->
## Find files modified after a specific date

```
find [directory path] -type f -newermt '[date and time]'
```

Example: find / -type f -newermt '6/30/2020 0:00:00' <br>
*(all dates/times after 6/30/2020 0:00:00 will be considered a condition to look for)* <br><br>

<!-- ----------------------------------------------- -->
## Find files based on date modified

```
find [directory path] -type f -newermt [start date range] ! -newermt [end date range]
```

Example: find / -type f -newermt 2013-09-12 ! -newermt 2013-09-14 <br>
*(all dates before 2013-09-12 will be excluded; all dates after 2013-09-14 will be excluded, therefore this only leaves 2013-09-13 as the date to look for.)* <br><br>

<!-- ----------------------------------------------- -->
## Find files based on date accessed

```
find [directory path] -type f -newerat [start date range] ! -newerat [end date range]
```

Example: find / -type f -newerat 2017-09-12 ! -newerat 2017-09-14 <br>
*(all dates before 2017-09-12 will be excluded; all dates after 2017-09-14 will be excluded, therefore this only leaves 2017-09-13 as the date to look for.)* <br><br>

<!-- ----------------------------------------------- -->
## Find files with a specific keyword

```
grep -iRl [directory path/keyword]
```

Example: grep -iRl '/folderA/flag' <br><br>

<!-- ----------------------------------------------- -->
## Filter your results to exclude files/directories that you do not have permission to

```
2>/dev/null
```
<br>

<!-- ----------------------------------------------- -->
## Find Manual

```
man find
```
<br>

<!-- ----------------------------------------------- -->
## Acknowledgments

* TryHackMe - Linux Strength Training (https://tryhackme.com/room/linuxstrengthtraining)
