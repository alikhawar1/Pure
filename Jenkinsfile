pipeline {
    agent { any 'node:6.9.5' }.git +refs/heads/master:refs/remotes/origin/master
Checking out Revision fc2d3bc6765b853732f334c3eb5808519ae36504 (master)
 > git config core.sparsecheckout # timeout=10
 > git checkout -f fc2d3bc6765b853732f334c3eb5808519ae36504
Commit message: "Update Jenkinsfile"
 > git rev-list --no-walk 0076aedb0f5d7d28e2d8ecfed77dc6353cad6326 # timeout=10
Cleaning workspace
    stages {
        stage('Build') {
            steps {
               echo 'npm install'
            }
        }
        stage('Test') {
           steps {
              sh 'npm test'
            }
        }
        
    }
}
