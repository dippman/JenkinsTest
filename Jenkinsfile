pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                bat 'print'
            }
        }
    }
    post{
             mail to: 'hoffmann4@wisc.edu',
             subject: "Failed Pipeline: ${currentBuild.fullDisplayName}",
             body: "asdfasdfgargf ${env.BUILD_URL}"
    }
}
