pipeline {
  agent any
  stages {
    stage('SonarQube analysis') {
      steps {
        sh '''steps {
    withSonarQubeEnv(\'SonarQube\') {
        sh \'mvn clean install sonar:sonar -Dsonar.host.url=http://localhost:8080 -Dsonar.login=admin\'
    }
}'''
        }
      }

    }
  }