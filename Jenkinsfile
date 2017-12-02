pipeline {
     agent any
     stages {
          stage("Compile") {
               steps {
                    sh "./mvnw compileJava"
               }
          }
          stage("Unit test") {
               steps {
					sh 'chmod +x mvnw'
                    sh "./mvnw test"
               }
          }
     }
}