# epam-training-ansible-new  

# Directory structure

.
├── hosts  
├── README.md  
├── roles  
│   ├── apache  
│   │   ├── handlers  
│   │   │   └── main.yml  
│   │   └── tasks  
│   │       └── main.yml  
│   ├── mysql  
│   │   └── tasks  
│   │       └── main.yml  
│   ├── php  
│   │   └── tasks  
│   │       └── main.yml  
│   └── wordpress  
│       ├── handlers  
│       │   └── main.yml  
│       └── tasks  
│           └── main.yml  
├── templates
│   └── apache.conf.j2  
├── vars  
│   └── default.yml  
└── wordpress.yml  

# Install Playbook  
Run ansible-playbook wordpress.yml -i hosts  

# Generate ssh key:  
Use private key for ansible SSH authentication  

ssh-copy-id -i ~/ssh/id_rsa.pub user@hostname
