

pipeline {
    agent any
    stages {
        stage('Build') { 
            steps {
                sh 'cd /opt/simple-java-maven-app && mvn -B -DskipTests clean package' 
            }
        }
    }
}


