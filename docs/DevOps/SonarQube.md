# SonarQube CheatSheet

1. Create Project
2. Click sur 'With GitLab CI'
3. Créer des variables d'intégration continue
    - Setting => CI / CD (Dans le projet GitLab)
    - Générer un token sur la page de SonarQube
    - Variables => Key = SONAR_TOKEN  Value = Value sur SonarQube
    - Variable => Key = SONAR_HOST_URL Value = Value sur SonarQube
4. Créer => `lvim sonar-project.properties` => Copier coller le code de SonarQube
5. Créer ou mettre à jour => `lvim .gitlab-ci.yml` => Copier coller le code de SonarQube
6. Faire une merge request pour que SonarQube se lance et affiche l'audit de code


## Le fichier .gitlab-ci
``` yaml
sonarqube-check:
  image:
    name: sonarsource/sonar-scanner-cli:latest
    entrypoint: [""]
  tags:
    - docker
  variables:
    SONAR_USER_HOME: "${CI_PROJECT_DIR}/.sonar" # Defines the location of the analysis task cache
    GIT_DEPTH: "0" # Tells git to fetch all the branches of the project, required by the analysis task
  cache:
    key: "${CI_JOB_NAME}"
    paths:
      - .sonar/cache
  script:
    - sonar-scanner
  allow_failure: true
  rules:
    - if: $CI_COMMIT_BRANCH == 'main'

```
