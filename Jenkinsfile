node {
   stage ('SCM Checkout') {
     git 'https://github.com/Fareeday/simple-java-maven-app.git'
                          }
   stage ('Compile-Package') {
     def mvnHome = tool name: 'Maven 4.0.0-alpha-13', type: 'maven'
     sh "${mvnHome}/bin/mvn package"
                             }
   stage ('Test') {
     def mvnHome = tool name: 'Maven 4.0.0-alpha-13', type: 'maven'
     sh "${mvnHome}/bin/mvn test"
                  }
    // post {
    //    always {
    //         junit 'target/surefire-reports/*.xml'
    //           }
    //      }
   stage ('Deliver') {
       sh './jenkins/scripts/deliver.sh'
                     }
     } 
