node {
   stage ('SCM Checkout') {
     git 'https://github.com/Fareeday/simple-java-maven-app.git'
  }
   stage ('Compile-Package') {
     sh 'mvn -B -DskipTests clean package'
  }
}


