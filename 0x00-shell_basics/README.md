# Shell Basics
> Tips for executing shell scripts
<!-- #### how to make a shell file executable. -->
```bash
 $ chmod u+x ./shell_file
```

0. #### How to see your absolute path of your current directory.
```bash
 $ pwd
 /home/remilekun/Documents/github/alx/alx-system_engineering-devops
```

1. #### how to list all files in a directory.
```bash
 $ ls
 ```

2. #### how to navigate to current users home directory.
```bash
 $ cd ~
 $ pwd
 # /home/remilekun
```

3. #### Display current directory contents in a long format
 ```bash
 $ ls -l
 ```

 4. #### Display current directory contents in a long format, including hidden files
```bash
$ ls -l -a
```

 5. #### Display current directory contents. 
 - Long format
 - with user and group IDs displayed numerically and hidden files (starting with .)
```bash
$ ls -l -a -n
```

6. #### Create a script that creates a directory named `my_first_directory` in the `/tmp/` directory.

```bash
$ mkdir /tmp/my_first_directory
```

7. #### Move the file betty from `/tmp/` to `/tmp/my_first_directory`.
```bash
$ mv /tmp/betty /tmp/my_first_directory/betty
```

8. #### Delete the file `betty`.
- The file betty is in /tmp/my_first_directory
```bash
$ rm /tmp/my_first_directory/betty
```

9. #### Delete the directory `my_first_directory` that is in the `/tmp` directory.
```bash
 $ rm -r /tmp/my_first_directory
```

10. Write a script that changes the working directory to the previous one.
> Before the task:
```bash
$ pwd
# /home/remilekun
$ ls
# Documents Downloads Pictures Public
cd Documents/github/alx
$ pwd
# /home/remilekun/Documents/github/alx
```
> Main task code
```bash
 $ cd -
# /home/remilekun
```

11. #### Write a script that lists all files (even ones with names beginning with a period character, which are normally hidden) in the current directory and the parent of the working directory and the `/boot` directory (in this order), in long format.
```bash
ls -la . .. /boot
# total 64
# drwxrwxr-x 2 remilekun remilekun 4096 Mar  3 21:34 .
# drwxrwxr-x 5 remilekun remilekun 4096 Mar  2 20:24 ..
# -rwxrw-r-- 1 remilekun remilekun   16 Mar  2 23:39 0-current_working_directory
```

12. #### Write a script that prints the type of the file named iamafile. The file iamafile will be in the `/tmp` directory when we will run your script.
```bash
file /tmp/iamafile
# /tmp/iamafile: ASCII text
```

13. #### Create a symbolic link to /bin/ls, named __ls__. The symbolic link should be created in the current working directory. 
```bash
ln -s /bin/ls __ls__
```
