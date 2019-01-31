# linux-useful-commands
## docker
display docker containers not wide terminal
```bash
docker ps | less -S
```
linux alias
```bash
alias l="ls -al"
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
