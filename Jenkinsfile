pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
              def mvnHome = tool name: 'Maven 4.0.0-alpha-13', type: 'maven'
              sh "${mvnHome}/bin/mvn package"
       }
      }
    }
  }

