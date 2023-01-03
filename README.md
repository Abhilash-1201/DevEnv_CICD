# DevEnv_CICD

Before Running the terraform file install terraform on the instance

Terraform Installation Steps:
------------------------------

##  First, install repository addition dependencies:

sudo apt update
sudo apt install  software-properties-common gnupg2 curl

## Now import repository GPG key

curl https://apt.releases.hashicorp.com/gpg | gpg --dearmor > hashicorp.gpg
sudo install -o root -g root -m 644 hashicorp.gpg /etc/apt/trusted.gpg.d/

## With the key imported now add Hashicorp repository to your Ubuntu system:

sudo apt-add-repository "deb [arch=$(dpkg --print-architecture)] https://apt.releases.hashicorp.com focal main"

## Now install terraform on your Ubuntu 22.04|20.04|18.04 system:

sudo apt update
sudo apt install terraform

## Check the version of terraform installed on your system

terraform --version

