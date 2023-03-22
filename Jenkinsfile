pipeline {
    agent any

    stages {
        stage ('Build') {
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

