## SonarQube Logs Volume

In the Docker Compose file, the `./sonarqube_logs` volume is mapped to `/opt/sonarqube/logs` inside the SonarQube container. This volume serves a crucial role:

- **Log Files**: All the SonarQube log files are stored in this directory. This includes logs of system events, analysis reports, and other activities.

- **Persistence**: The `./sonarqube_logs` volume is crucial for persisting logs between SonarQube container restarts or updates. Without this persistence, all SonarQube logs would be lost each time the SonarQube container is restarted or updated.