# Guide to setup docker environment

1. Login as root user by doing sudo bash or use sudo before each command
2. Clone this repo in /opt directory.
3. Assuming, docker engine is installed, if not follow these steps:

# Install docker engine
```
sudo apt-get update
sudo apt-get install apt-transport-https ca-certificates -y
sudo apt-key adv --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 58118E89F3A912897C070ADBF76221572C52609D
sudo apt-add-repository 'deb https://apt.dockerproject.org/repo ubuntu-trusty main'      # For Ubuntu 14.04
sudo apt-add-repository 'deb https://apt.dockerproject.org/repo ubuntu-xenial main'     # For Ubuntu 16.04
sudo apt-get update
sudo apt-get install docker-engine -y
```

# Install Docker Compose:
```
apt-get install python-pip -y
export LC_ALL=C   # If Server Throws Exception
pip install docker-compose
```
4. Under /opt/demo directory run:
```
docker-compose up -d
```

5. Make sure these ports are open in firewall: 80, 4001, 5001, 8080
6. In index.html file under html folder, change in line 15: Update the url accordigly.
