

pipeline {
    agent any
    stages {
        stage('Build') { 
            steps {
                def mvnHome = tool name: 'Apache Maven 3.6.0', type: 'maven'
                sh 'mvn -B -DskipTests clean package'
            }

        }
    }
}


