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
             mail to: 'hoffmann4@wisc.edu',
             subject: "Failed Pipeline: ${currentBuild.fullDisplayName}",
             body: "asdfasdfgargf ${env.BUILD_URL}"
        }
    }
}
