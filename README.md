<!--
chmod 400 "s.pem"
ssh -i "s.pem" ubuntu@ec2-35-159-7-150.eu-central-1.compute.amazonaws.com
sudo apt update
sudo apt install nginx -y
sudo systemctl start nginx
sudo systemctl enable nginx
sudo systemctl status nginx
sudo apt install git -y
cd /var/www/html
ls
sudo rm -rf /var/www/html/*
sudo git clone https://github.com/AsleshaPS/static_website.git /var/www/html
sudo systemctl reload nginx
http://<ip> 

sec rules->port(src)=3000
http://<ip>:3000
python3 -m http.server 3000 
-->

<!--
create 2 instances
security->security grps->edit inbound rules
    add rule all icmp ipv4
chmod 400 vm.pem
ssh -i vm.pem ubuntu@SENDER PUBLIC IP
ping RECEIVER PRIVATE IP
nano file.txt
from 2nd terminal-
    scp -i vm.pem vm.pem ubuntu@SENDER PUBLIC IP:/home/ubuntu/
in 1st terminal-
    chmod 400 vm.pem
    scp -i vm.pem file.txt ubuntu@RECEIVER PRIVATE IP:/home/ubuntu/
in 3rd terminal-
    ssh −i vm.pem ubuntu@RECEIVER PUBLIC IP
    ls
    cat file.txt
-->

<!--
git clone https://github.com/rishipalkar/aws-blog-app.git
cd aws-blog-app
sudo apt update
sudo snap install docker
sudo docker compose up -d
sudo docker compose build --no-cache frontend 
-->
