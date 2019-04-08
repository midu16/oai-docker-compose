# Docker-compose.yml to deploy a chain settup of dockers
# file          README
# author        Mihai IDU (C) - 2019 

**WARNING NOTE**: This will create a container with **security** options **disabled**, this is an unsupported setup, if you have multiple snap packages inside the same container they will be able to break out of the confinement and see each others data and processes.


```
Content:
├── db-node
│   └── db-dockerfile
├── docker-compose.yml
├── LICENSE
├── prepare_the_environment
├── README.md
└── ubuntu-node
    └── ubuntu-dockerfile
```
After building the docker-compose model there will be available the following:
```
cigarier@cigarier:~/oai-docker-compose$ sudo docker images
REPOSITORY                TAG                 IMAGE ID            CREATED             SIZE
oaidockercompose_ubuntu   latest              cc665fb384f3        2 hours ago         343MB
mysql                     5.7                 98455b9624a9        12 days ago         372MB
ubuntu                    16.04               9361ce633ff1        3 weeks ago         118MB
phpmyadmin/phpmyadmin     latest              c6ba363e7c9b        2 months ago        166MB

The images are available also on the https://hub.docker.com/ 
```

**NOTE:** That the GTP kernel should be enable on the hoast machine.

```
uname -a
sudo modprobe gtp
dmesg |tail # You should see something that says about GTP kernel module
```

