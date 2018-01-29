pipeline {
    agent { any 'node:6.9.5' }
    stages {
        stage('build') {
            steps {
                sh 'npm install'
                sh 'npm rebuild'
            }
        stage('test') {
                sh 'npm test'
        }
       }
    }
}
