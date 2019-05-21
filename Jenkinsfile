pipeline {
   agent any
   stages{
     stage('Build') { 
         steps {
             sh '/usr/local/maven/bin/mvn clean package'
             sh "docker build . -t tomcapwebbapp:${env.BUILD_ID}"
         }
     }
   }
}
