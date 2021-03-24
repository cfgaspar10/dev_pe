Docker RHSISPEN APACHE/PHP/PHPMYADMIN/MARIADB versão desenvolvimento
=========
   
   ### Instalação Docker
   
   $ sudo apt-get update
   
   $ sudo apt install docker.io
   
   $ sudo systemctl start docker
   
   $ docker --version
   
   $ sudo systemctl enable docker
   
   $ sudo docker run hello-world
   
   ### Instalação docker-compose
   
   $ sudo apt-get update
   
   $ sudo curl -L https://github.com/docker/compose/releases/download/1.25.3/docker-compose-`uname -s`-`uname -m` -o /usr/local/bin/docker-compose
   
   $ sudo chmod +x /usr/local/bin/docker-compose
   
   $ sudo docker-compose --version
   
=========
   
    #Passos para executar a composição dos containers
    $ git clone https://github.com/cfgaspar10/dev_pe.git
    $ cd dev_pe  
    $ sudo docker-compose up -d --build
    $ sudo docker ps(para verificar os containers em execução)
    
    ### Acessar Container "www".
    $ sudo docker exec -ti docker_dev_pe_www_1 /bin/bash
    ### Acessar Container "db".
    $ sudo docker exec -ti docker_dev_pe_db_1 /bin/bash
     ### Acessar Container "phpmyadmin".
    $ sudo docker exec -ti docker_dev_pe_phpmyadmin_1 /bin/bash
     
    Browser Servidor -> [http://localhost:8084/)
    Browser phpMyAdmin -> [http://localhost:8085]
  
=========

