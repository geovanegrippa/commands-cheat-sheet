# Container Operations  
- `docker ps`                          // List running containers  
- `docker ps -a`                       // List all containers  
- `docker start/stop <container>`      // Start/Stop container  
- `docker restart <container>`         // Restart container  
- `docker exec -it <container> bash`   // Enter container shell  
- `docker rm <container>`              // Remove container  
- `docker rename <old> <new>`          // Rename container  
  
# Image Operations  
- `docker images`                      // List all images  
- `docker pull <image>`                // Download image  
- `docker build -t <name> .`           // Build image from docker file  
- `docker rmi <image>`                 // Remove image  
- `docker history <image>`             // Show image history  
  
# Run Containers  
- `docker run --name nginx-test -d -p 8080:80 nginx`  // Executa o NGINX em modo destacado e mapeia porta 80 para 8080  
- `docker run --rm busybox echo "Hello from BusyBox"`  // Executa um comando simples no BusyBox e remove o container ao finalizar  
- `docker run -it --rm busybox sh`                   // Abre um shell interativo no BusyBox e exclui ao sair  
  
# Network Operations  
- `docker network ls`                  // List all networks  
- `docker network inspect <network>`   // Show network details  
- `docker network create <name>`       // Create network  

# Volume Operations  
- `docker volume ls`                   // List volumes  
- `docker volume create <name>`        // Create volume  
- `docker volume inspect <name>`       // Inspect volume  
- `docker volume rm <name>`            // Remove volume  
  
# Logs & Monitoring  
- `docker logs -f <container>`         // Follow container logs  
- `docker stats`                       // Show resource usage  
- `docker inspect <container>`         // Container details  
- `docker top <container>`             // Show running processes  
  
# Docker Compose  
- `docker-compose up -d`               // Start services in background  
- `docker-compose down`                // Stop and remove services  
- `docker-compose ps`                  // List services  
- `docker-compose logs -f`             // Follow service logs  


