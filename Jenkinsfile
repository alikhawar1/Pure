pipeline {
    agent { any 'node:6.9.5' }
    stages {
        stage('Build') {
            when {
    branch 'master'
}
            steps {
               echo 'npm install'
            }
        }
        stage('Test') {
             when {
        expression { return params.enableDps }
    }


           steps {
                 timeout(time: 10, unit: 'HOURS') {
            ecdmItestRun(
                vmIp : "${params.vmIp}",
                itestPath : "itests/restapi/dps",
                itestName : "DPS",
                additionalArgs : "-Prun-its,run-its-irvine"
                )
        }
               echo 'chmod +x test'
              
            }
        }
        
    }
}
