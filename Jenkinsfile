pipeline {
    agent { any 'node:6.9.5' }
    stages {
        stage('Build') {
            steps {
                sh 'npm install'
                sh ' npm test'
            }
        }
       // stage('Test') {
         //   steps {
           //     sh 'npm test'
            //}
        //}
        
    }
}
