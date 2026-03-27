pipeline {
    agent any 
    stages {
       stage('Build') {
           steps {
               sh 'docker-compose build'
           }
       }
       stage('Stop Old Containers') {
           steps {
               sh 'docker-compose down' 
           }
       }
       stage('Start New Containers') {
           steps {
               sh 'docker-compose up -d'
               }
           }
     }
} 
