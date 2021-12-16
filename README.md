# Docker images
Images for docker if you cannot pull images from docker hub.

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


