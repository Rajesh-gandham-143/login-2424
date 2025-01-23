pipeline {
    agent any 
    stages{
        stage('deploy') {
            steps{
                sh 'rm -rf /var/www/html/*'
                sh 'cp -r . /var/www/html'
            }

        }
        stage('info') {
            steps{
                sh 'df -h'
                sh 'free -h'
            }
        }
    }
    
}