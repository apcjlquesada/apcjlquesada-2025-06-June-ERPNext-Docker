# apcjlquesada-2025-06-June-ERPNext-Docker

https://codewithkarani.com/2024/04/06/installing-erpnext-via-docker-for-beginners-a-step-by-step-guide/ 


On github.com 
1. Create a new repository 
2. Start a Codespace 
3. Follow codewithkarani steps.


- docker compose -p pwd -f docker-compose.yml up

# Steps  to log into the Frappe Backend Docker container 
- docker ps -a
- look for the ID of  (pwd-backend-1)
- Replace 'ID' with the ID of  (pwd-backend-1)
- sudo docker exec -it 'ID' /bin/bash

