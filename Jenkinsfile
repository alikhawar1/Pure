pipeline {
    agent { any 'node:6.9.5' }
    stages {
        stage('Build') {
            steps {
               echo 'npm install'
            }
        }
        stage('Test') {
           steps {
               sh 'chmod +x index.js'
              sh './index.js'
            }
        }
        
    }
}
