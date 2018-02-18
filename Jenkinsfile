pipeline {
    agent { any 'node:6.9.5' }
    stages {
        stage('Build') {
            when {
    branch 'develop'
}
            steps {
               sh 'npm install'
            }
        }
        stage('Test') {


           steps {
               echo 'chmod +x test'
              
            }
        }
        
    }
}
