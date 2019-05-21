pipeline {
   agent any
   stages{
     stage('Build') { 
         steps {
             sh 'id'
             sh 'mvn clean package'
             sh "docker build . -t tomcapwebbapp:${env.BUILD_ID}"
         }
     }
   }
}
