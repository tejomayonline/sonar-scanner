# sonar-scanner
Sonar Scanner with SonarQube and Postgres

#### Steps to run sonar scanner locally
- `docker-compose up -d` to run sonar scanner.
-  check `http://localhost:9000` for the sonar admin panel.
-  default username `admin` and password is `bitnami`.

#### Steps to scan by sonar scanner locally
- go to project root and run `sonar-scanner -Dsonar.login=YOUR_SONAR_LOGIN_ID -Dsonar.password=YOUR_SONAR_LOGIN_PASSWORD`. (Note: the project to scan should have `sonar.properties` file or need to put manually during runtime.)
- On successful completion goto the sonar portal. The Project will be added.

Inspired from `https://github.com/bitnami/bitnami-docker-sonarqube`
