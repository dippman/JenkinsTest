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
         stage('Deploy'){
            steps {
                  
                  }
            }
         }
    post{
        always{
             echo("Pipeline is correct")
        }
    }
        
}
