pipeline {
  agent any
  stages {
    stage('SonarQube analysis') {
      steps {
        sh '''pipeline {
    agent any

    tools {
        // Install Maven and add it to the path.
        maven "maven"
    }

    stages {
        stage(\'SonarQube Analysis\') {
            steps {
                // Analyze the code with SonarQube
                withSonarQubeEnv(\'My SonarQube Server\') {
                    sh "mvn sonar:sonar"
                }
            }
        }
    }
}
'''
        }
      }

    }
  }