pipeline {
    agent any
    stages {
        stage('SCM Checkout') { 
            steps {
                git 'https://github.com/Fareeday/simple-java-maven-app.git' 
            }
        stage('Build') {
            steps {
                sh 'mvn -B -DskipTests clean package' 
        }
      }
    }
  }
}

