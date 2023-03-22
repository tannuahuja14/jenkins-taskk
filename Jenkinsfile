pipeline {
  agent any
    stages {
        stage ('Development') {
            steps {
                sh '''
                javac sum.java
                java sum
                '''
                echo "Build Successful."
            }
        }
    }
}

