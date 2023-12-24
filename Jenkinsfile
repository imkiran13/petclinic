pipeline {
    agent any
    
   tools{
       jdk 'jdk-17'
       maven 'maven'
   }
    stages {
        stage('checkout') {
            steps {
               git branch: 'main', url: 'https://github.com/imkiran13/petclinic.git'
            }
        }
        
         stage('compile') {
            steps {
              sh "mvn clean compile"
            }
        } 
        
        stage('build') {
            steps {
              sh "mvn clean package"
            }
        }
        
         
    }
}
