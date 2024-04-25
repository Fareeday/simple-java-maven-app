

pipeline {
    agent any
    stages {
        stage('Build') { 
            steps {
                sh "${MVN}/bin/mvn -B -DskipTests clean package"
            }
        }
    }
}


