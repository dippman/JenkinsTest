pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                bat 'set'
            }
        }
                  stage('test'){
       steps {
             input "Does the staging environment look ok?"
             }
                  }
    }
    post{
        always{
             echo("Pipeline:" + ${currentBuild.fullDisplayName})
        }
    }
        
}
