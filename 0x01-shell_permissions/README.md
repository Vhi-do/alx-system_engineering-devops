## Hello world
0. #### Change current user to `betty`
```bash
$ su betty
```

1. #### how to know the current user
```bash
$ whoami
# betty
```

2. #### list the groups that the current user belongs to
```bash
$ groups
# adm dialout cdrom floppy audio video plugdev users
```

3. #### Change the owner of the file `hello` to `betty`
```bash
$ chown betty ./hello
```

4. #### Create a file `hello`
```bash
$ touch hello
```

5. #### Write a script that adds execute permission to the owner of the file hello.
- The file `hello` will be in the working directory
```bash
$ chmod 744 ./hello
```

6. #### Write a script that adds execute permission to the owner and the group owner, and read permission to other users, to the file `hello`
```bash
$ chmod 554 ./hello
```

7. #### Write a script that adds execution permission to the owner, the group owner and the other users, to the file hello
- The file hello will be in the working directory
- You are not allowed to use commas for this script
```bash
$ chmod a+x ./hello
```