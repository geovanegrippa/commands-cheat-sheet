# Comandos Básicos Linux

## Arquivos e Navegação
- `ls` - directory listing (list all files/folders on current dir)  
- `ls -l` - formatted listing  
- `ls -la` - formatted listing including hidden files  
- `cd dir` - change directory to dir (dir will be directory name)  
- `cd ..` - change to parent directory  
- `cd ~` - change to home directory  
- `pwd` - show current directory  
- `mkdir dir` - create a directory dir  
- `rm file` - delete file  
- `rm -f file` - force remove file  
- `rm -r dir` - delete directory dir  
- `rm -rf dir` - remove directory dir  
- `rm -rf /` - launches some nuclear bombs targeting your system  
- `cp file1 file2` - copy file1 to file2  
- `mv file1 file2` - move file1 to file2  
- `mv file1 dir/file2` - move file1 to dir as file2  
- `touch file` - create or update file  
- `cat file` - output contents of file  
- `cat file1 file2 > file3` - combine file1 and file2 into file3  
- `cat >> file` - append standard input into file  
- `tail -f file` - output contents of file as it grows  

## Redes
- `ping host` - ping host  
- `whois domain` - get whois for domain  
- `dig domain` - get DNS for domain  
- `host host` - resolve lookup host  
- `wget file` - download file  
- `wget -c url` - continue stopped download  
- `wget -r url` - recursively downloads files form url  
- `curl url` - output webpage content as plain text  
- `curl -o meuhmtl url` - writes page to meh.html  
- `ssh user@host` - connect using ssh  
- `ssh -p port user@host` - connect using port  

## Processos
- `ps` - display currently active processes  
- `ps aux` - detailed outputs  
- `kill pid` - kill process with process id (pid)  
- `killall proc` - kill all processes named proc  

## Informações de Sistema
- `date` - show current date/time  
- `uptime` - show uptime  
- `whoami` - who you logged in as  
- `w` - display who is online  
- `cat /proc/cpuinfo` - display cpu info  
- `cat /proc/meminfo` - memory info  
- `free` - show memory and swap usage  
- `du` - show directory space usage  
- `du -sh` - displays readable sizes in GB  
- `df` - show disk usage  
- `uname -a` - show kernel config  

## Compressão
- `tar cf file.tar files` - tar files into file.tar  
- `tar xf file.tar` - untar into current directory  
- `tar tf file.tar` - show contents of archive  

### Options
- `c` - create archive  
- `t` - table of contents  
- `x` - extract  
- `z` - use zip/gzip  
- `f` - specify filename  
- `j` - bzip2 compression  
- `w` - ask for confirmation  
- `k` - do not overwrite  
- `X` - files from file  
- `v` - verbose  

## Permissões
- `chmod octal file` - change permissions of file  

### Octal Values
- 4 = read (r)  
- 2 = write (w)  
- 1 = execute (x)  

Order: owner/group/world  

Exemplos:  
- `chmod 777` - rwx for everyone  
- `chmod 755` - rwx for owner, rx for group world  

## Outros
- `grep pattern files` - search in files for pattern  
- `grep -r pattern dir` - search for pattern recursively in dir  
- `locate file` - find all instances of file  
- `whereis app` - show possible locations of app  
- `man command` - show manual page for command  
