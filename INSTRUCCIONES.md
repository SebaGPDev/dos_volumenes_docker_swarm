# Desplegar dos servicios con Docker Swarm- volumenes

### Crear las imagenes en base al dockerfile correspondiente a cada carpeta
docker build -t tp2/php .
docker build -t tp2/node .
docker build -t tp2/mysql .

### Iniciar swarm
docker swarm init

### Se despliega una pila de servicios en base al docker-compose
docker stack deploy -c docker-compose.yml mis-servicios


