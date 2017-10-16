sudo apt-get install docker
sudo apt install docker.io

cd /home/carlvdl/IdeaProjects/docker_nodejs
sudo docker build -t carlvdl/docker_nodejs .

sudo docker run -p 49160:8080 -d carlvdl/docker_nodejs
sudo docker ps
curl -i localhost:49160
