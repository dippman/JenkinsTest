pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                bat 'set'
            }
        }
    }
    post{
        always{
             echo("Pipeline:" + ${currentBuild.fullDisplayName})
        }
    }
                  stage('test'){
                       steps {
                    input "Does the staging environment look ok?"
            }
                  }
}
