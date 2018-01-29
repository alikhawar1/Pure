pipeline {
    agent { any 'node:6.9.5' }
    stages {
        stage('Build') {
            steps {
                sh 'npm install'
            }
        }
        stage('Test') {
            steps {
                echo 'npm test'
            }
        }
        
    }
