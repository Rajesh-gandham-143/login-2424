pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'cat /os/releases'
            }
        }
        stage('Test') {
            steps {
                sh 'df -h'
            }
        }
        stage('Deploy') {
            steps {
                sh 'free '
            }
        }
    }
}