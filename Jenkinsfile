pipeline {
  agent any
    stage('git checkout'){
    git credentialsId: 'gitcheckout2', url: 'https://github.com/vamshima/getting-started.git'
               } 
  
    stage('Docker Build') {
      steps {
        sh 'docker build -t shanem/spring-petclinic:latest .'
      }
    }
}
