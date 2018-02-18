pipeline {
    agent { any 'node:6.9.5' }
    stages {
        stage('Build') {
            when {
    branch 'develop'
}
            steps {
               sh "bower install"
                sh "npm install"
                sh "npm build"
            }
        }
        stage('Test') {


           steps {
               echo 'chmod +x test'
              
            }
        }
        
    }
}
