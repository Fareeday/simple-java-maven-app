node {
   stage ('SCM Checkout') {
     git 'https://github.com/Fareeday/simple-java-maven-app.git'
  }
   stage ('Compile-Package') {
     def mvnHome = tool name: 'Maven 4.0.0-alpha-13', type: 'maven'
     sh '${mvnHome}/bin/mvn package'
  }
}


