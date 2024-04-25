pipeline {
    agent any
    stages {
        stage('SCM Checkout') { 
            steps {
                git 'https://github.com/Fareeday/simple-java-maven-app.git' 
            }
        stage('Build') {
               def mvnHome = tool name: 'Maven 4.0.0-alpha-13', type: 'maven'
               sh "${mvnHome}/bin/mvn package"
      }
    }
  }
}

