pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                bat 'set'
                //bat 'javac HelloWorld.java java HelloWorld'
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
