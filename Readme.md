to run this microservices project in ec2 amazon Linux follow below steps


step: sudo yum update -y
step: sudo yum install docker -y
step: sudo systemctl start docker
step: sudo systemctl enable docker
step: sudo docker --version
step: sudo curl -L "https://github.com/docker/compose/releases/download/v2.27.1/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
step: sudo chmod +x /usr/local/bin/docker-compose
step: sudo docker-compose version
step: sudo yum install git -y
step: git version
step: git clone https://github.com/shahrukhkh/microservices.git
step: cd microservices/
step: sudo docker-compose up -d
step: sudo docker ps
step: sudo docker images
step: sudo docker logs config-server  OR sudo docker logs config-server -f
step: http://<your-ip>:8080/order-ms/order/msg


