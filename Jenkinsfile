

pipeline {
    agent any
    stages {
        stage('Build') { 
            steps {
                sh '${mvnHome}/bin/mvn -B -DskipTests clean package'
            }
        }
    }
}


