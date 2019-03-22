# linux-useful-commands

# docker
display docker containers not wide terminal
```bash
docker ps | less -S
```
get ip of all running containers
```
docker inspect -f '{{.Name}} - {{range .NetworkSettings.Networks}}{{.IPAddress}}{{end}}' $(docker ps -aq)
```

# git useful commands
create a branch from a specific commit
```bash
git checkout commit_id
git checkout -b new_branch_name
git push -u origin new_branch_name
```
pull from a another branch - only specific commit
```bash
git cherry-pick <commit-hash>
```

# general commands
copy files from server A to B (remote)
```bash
scp -r -i  ~/.ssh/key.pem /home/user/Desktop/source/  user@host_address:/var/www/destination/path
```
copy files from server B (remote) to A
```bash
scp -r user@host_address:/var/www/source /home/user/Desktop/
```
copy files from server A to B (remote) using rsync and pem key for ssh
```
rsync -avh -e "ssh -i ~/.ssh/example.pem" /home/user/Desctop/source root@192.168.0.100::/var/www/destination/path
```


querying DNS
```bash
dig example.com
```
linux alias
```bash
alias l="ls -al"
```
