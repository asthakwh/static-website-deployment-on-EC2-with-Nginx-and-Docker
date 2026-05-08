step 1 install docker

    sudo apt update && sudo apt upgrade  -y
    sudo apt install docker.io -y
    sudo systemctl start docker
    sudo systemctl enable docker
    sudo systemctl status docker
    install Docker on your system

step 2 install nginx

    sudo apt update && sudo apt install -y nginx && nginx -v && sudo systemctl enable --now nginx
    sudo systemctl status nginx

step 3 create files

    mkdir host-web
    cd host-web
    ls
    vi index.html
    Vi Dockerfile

step 4 run container

    sudo docker build -t demo-website .
    sudo docker run -d -p 8080:80 demo-website
    sudo curl http://52.66.244.97:8080/

step 5 check on your browser
