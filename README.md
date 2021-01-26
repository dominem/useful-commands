# useful-commands

## GIT

Grep through repo's history:

```
git grep <regexp> $(git rev-list --all)
```

Grep through file's history:

```
git grep <regexp> $(git rev-list --all -- <file>) -- <file>
```

## Linux

Background task:

```
setsid COMMAND &
```

https://man7.org/linux/man-pages/man1/setsid.1.html  
https://www.ibm.com/support/pages/nohup-or-setsid-keep-process-running-after-user-disconnect  
https://unix.stackexchange.com/a/352923  

Redirection (both stdout & stderr):

```
command &> file
```

https://askubuntu.com/a/731237  

Restricting Process CPU Usage:

```
nice COMMAND
```

https://scoutapm.com/blog/restricting-process-cpu-usage-using-nice-cpulimit-and-cgroups  

`setsid` + `nice` + stdout/stderr redirection:

```
setsid nice COMMAND &> out.txt &
```
