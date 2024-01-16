## Website tester 

This website tester uses Jenkins and Sonarqube with Databases linked in the container. The data is persistant after stop and is kept in the directory. 

# Installation Instructions

1. Clone the repository
```bash
  git clone git@github.com:UnMugViolet/website-tester.git
```
   
3. Navigate to the cloned repository
```bash
  cd website-tester/
```
   
5. Create the necessary directories:
```bash
mkdir jenkins_home mariadb_data postgres_data sonarqube_data sonarqube_extensions sonarqube_logs
```
6. Build the container
```bash
docker compose up -d 
```
