pipeline {
  agent any
    stages {
        stage ('Development') {
            steps {
                sh '''
                javac Sum.java
                java Sum
                '''
                echo "Build Successful."
            }
        }
    }
   post {
           failure {
               emailext attachLog:true, body: 'Pipeline is failed!', subject: 'Post Build Action Email', to: 'tannu.ahuja@knoldus.com'
        }
}

