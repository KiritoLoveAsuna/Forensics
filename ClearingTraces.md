### Linux
###### Shredding files
shred(kali) -f -n 3 filepath  

###### clear bash history
1. history -c(clear the history on the current BASH shell)
2. export HISTSIZE=0
3. history -w(only clears the history of the current shell)
4. cat /dev/null > ~.bash_history && history -c && exit
5. shred ~/.bash_history
6. shred ~/.bash_history && cat /dev/null > .bash_history && history -c && exit  

### Windows
###### Windows Clearing Logs
```
获取日志分类列表：
wevtutil el >1.txt

获取单个日志类别的统计信息：
wevtutil gli "windows powershell"

回显：
creationTime: 2016-11-28T06:01:37.986Z
lastAccessTime: 2016-11-28T06:01:37.986Z
lastWriteTime: 2017-08-08T08:01:20.979Z
fileSize: 1118208
attributes: 32
numberOfLogRecords: 1228
oldestRecordNumber: 1

查看指定日志的具体内容：
wevtutil qe /f:text "windows powershell"

删除单个日志类别的所有信息：
wevtutil cl "windows powershell"
```
