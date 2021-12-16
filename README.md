# Docker images
Images for docker if you cannot pull images from docker hub.


## Start a mssql-server instance running as the SQL Express edition
mssqlexpress.rar is the backup of mssql express server
sudo docker load -i mssqlexpress.rar
docker run -e "ACCEPT_EULA=Y" -e "SA_PASSWORD=yourStrong(!)Password" -e "MSSQL_PID=Express" -p 1433:1433 -d mcr.microsoft.com/mssql/server:2019-latest 


## Backup
sudo docker save -o ~/my-backup.tar my-backup
## Restore
sudo docker load -i ~/my-backup.tar


## How to upload big files to github
curl -s https://packagecloud.io/install/repositories/github/git-lfs/script.deb.sh | sudo bash

sudo apt-get install git-lfs

git lfs install

git lfs track '*.rar'

git lfs push --all origin master

git push -u origin master


