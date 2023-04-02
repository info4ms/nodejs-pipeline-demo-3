pipeline {
  agent any
    
  tools {nodejs "node"}
    
  stages {
        
    stage('Git') {
      steps {
        git 'https://github.com/info4ms/nodejs-pipeline-demo-3.git'
      }
    }
     
    stage('Build') {
      steps {
        sh 'npm install'
         echo '<<Build Command>>'
      }
    }  
    
            
    stage('Test') {
      steps {
        sh 'node test'
      }
    }
  }
}
