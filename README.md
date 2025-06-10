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

# Installing A Custom App On Your Running ERPNext Instance Installed via Docker
https://codewithkarani.com/2024/04/06/installing-a-custom-app-on-your-running-erpnext-instance-installed-via-docker/ 
- sudo docker exec -it <NAME> /bin/bash
- git clone <repository_url>
- bench --site <site_name> install-app <app_name>
- bench --site <site_name> migrate

# Installing healthcare app

https://github.com/earthians/marley/tree/version-15

- bench get-app healthcare --branch version-15
- bench --site frontend install-app healthcare
- bench --site frontend migrate


# Installing HRMS app
- bench get-app hrms  --branch version-15
- bench --site frontend install-app hrms
- bench --site frontend migrate

# Other bench commands
- bench --site frontend list-apps
