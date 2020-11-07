pipeline {
 agent any
 stages
 {
  stage('Checkout')
  {
   steps { 
    git branch: 'master', url: 'https://github.com/joshna1926/maven-web-application.git'
     }
  }
  agent any  
    stages { 
        stage('Build') { 
            steps { 
               sh "mvn clean package"
            }
        }
    }
 }
}


 
