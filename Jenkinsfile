pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                bat 'set'
                javac Hello.java java Hello
            }
        }
         stage('test'){
            steps {
                 input "Does the staging environment look ok?"
                  }
            }
         stage('Deploy'){
            steps {
                  echo 'deploy...'
                  }
            }
         }
    post{
        always{
             echo("Pipeline is correct")
        }
    }
        
}
