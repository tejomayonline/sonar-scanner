# sonar-scanner
Sonar Scanner with SonarQube and Postgres

#### Prerequisite
- download sonar-scanner from `https://docs.sonarqube.org/latest/analysis/scan/sonarscanner`
- update system path variable with sonar-scanner/bin dir. Add `export PATH="/Users/YOUR_USER/sonar-scanner-4.0.0.1744-macosx/bin:$PATH"` to bash ( i.e .bash_aliases/ .bash_profile/ .bashrc).
- now try sonar-scanner command.

#### Steps to run sonar scanner locally
- `docker-compose up -d` to run sonar scanner.
-  check `http://localhost:9000` for the sonar admin panel.
-  default username `admin` and password is `bitnami`.

#### Steps to scan by sonar scanner locally
- go to project root and run `sonar-scanner -Dsonar.login=YOUR_SONAR_LOGIN_ID -Dsonar.password=YOUR_SONAR_LOGIN_PASSWORD`. (Note: the project to scan should have `sonar.properties` file or need to put manually during runtime.)
- On successful completion goto the sonar portal. The Project will be added.

Inspired by `https://github.com/bitnami/bitnami-docker-sonarqube`
