pipeline {
   agent any
   stages{
     stage('Build') { 
         steps {
             sh 'source /etc/profile'
             sh 'id'
             sh '/usr/local/maven/bin/mvn clean package'
             sh "docker build . -t tomcapwebbapp:${env.BUILD_ID}"
         }
     }
   }
}
