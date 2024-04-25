

pipeline {
    agent any
    stages {
        stage('Build') { 
            steps {
                sh 'cd /opt/simple-java-maven-app && sudo -u root mvn -B -DskipTests clean package'
            }
        }
    }
}


