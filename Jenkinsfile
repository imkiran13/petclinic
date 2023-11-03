pipeline {
    agent any
    
   tools{
       jdk 'jdk-11'
       maven 'maven-3'
   }
    stages {
        stage('checkout') {
            steps {
               git branch: 'feature-1', url: 'https://github.com/imkiran13/petclinic.git'
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
