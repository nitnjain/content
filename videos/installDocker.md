### Steps to install Docker on Ubuntu 20.04 (focal)

1) Update your apt lists.

`sudo apt update`

2) Install some packages which will help us install docker.

`sudo apt install ca-certificates apt-transport-https software-properties-common curl`

3) Download the Docker repository gpg key and add it to apt so that we apt can verify that the repo that we tell apt to add to the list is secure.

`curl -fsSl https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -`

4) Add the official Docker repository link to apt so that we can download the official Docker packages.

`sudo add-apt-repository "deb https://download.docker.com/linux/ubuntu focal stable`

5) Update the apt lists again.

`sudo apt update`

6) Install docker-ce, this will install docker and start running it.

`sudo apt install docker-ce`

7) Verify that docker is running by running:

`sudo systemctl status docker`

It should say somewhere *ACTIVE (running)* which will tell you that Docker is successfully installed and running.

Video Link: https://youtu.be/7EFlEY83zBY
