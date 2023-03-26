pipeline {
    agent any
  
    stages {
        stage('Fetch code') {
            steps {
                git branch: 'paac', url: 'https://github.com/dineshtamang14/DevOps-Course.git'
            }
        }
        
        stage('Build') {
            options {
               skipDefaultCheckout()
            }
            
            steps {
                sh 'mvn install'
            }
        }
        
        stage('test'){
            steps {
                sh 'mvn test'
            }
        }
    }
}
