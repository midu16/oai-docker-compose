Docker-compose.yml to deploy a chain settup of dockers

# file          README
# author        Mihai IDU (C) - 2019 mihai.idu@eurecom.fr

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

