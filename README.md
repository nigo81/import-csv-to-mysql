# import-csv-to-mysql
import csv or txt files to mysql.

[中文说明](./README_CN.md) 

[视频介绍](https://www.bilibili.com/video/BV1HS4y1m748/) 

## how to install

clone the project:

```bash
git clone https://github.com/nigo81/import-csv-to-mysql.git
```

prompt the `csv2mysql` execute privileges

```bash
chmod +x csv2mysql
```

cp `csv2mysql` to `~/.local/bin`:

```bash
cp csv2mysql ~/.local/bin
```

at first you shoule install `fzf` which is a file search tool in linux.

## how to use

change to the directory where your csv files are, and execute `csv2mysql`


![fzf](pictures/fzf.png)

your can use `fzf` to search file, type `tab` to select your data files.

finished with `enter`.

![shell](pictures/shell.png)

```bash
    ~/tmp  csv2mysql
input some database parameters

Enter your host ip,(default is 127.0.0.1)🔗:
Enter your database name 📚:book
Enter your account name 🥷:root
Enter password 🔑:\n
table name 📑:vip
do your wan't to drop table if exists? 0:don't drop, 1:drop  :1
data ignore lines num,usually as 0 or 1:1
input character set（default is utf8):
```

your should input your mysql datase info, such as `ip`,`database name`,`account`,`password`.

you should input `table name`, which the table your data will store in.(it will auto create table,if not exists)

