## SonarQube Extensions Volume

In the Docker Compose file, the `./sonarqube_extensions` volume is mapped to `/opt/sonarqube/extensions` inside the SonarQube container. This volume serves a crucial role:

- **Extensions Files**: All the SonarQube extensions files are stored in this directory. This includes plugins and other extensions.

- **Persistence**: The `./sonarqube_extensions` volume is crucial for persisting extensions between SonarQube container restarts or updates. Without this persistence, all SonarQube extensions would be lost each time the SonarQube container is restarted or updated.
