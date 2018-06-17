```bash
sudo apt update
sudo apt install curl
sudo apt-get install lsb-release

AZ_REPO=$(lsb_release -cs)
echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" | \sudo tee /etc/apt/sources.list.d/azure-cli.list

curl -L https://packages.microsoft.com/keys/microsoft.asc | sudo apt-key add -

sudo apt-get install apt-transport-https
sudo apt-get update && sudo apt-get install azure-cli

sudo apt-get update
sudo apt-get upgrade
sudo apt-get install git
```