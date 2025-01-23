pipeline {
    agent any 
    stages{
        stage('deploy') {
            steps{
                sh 'rm -rf /var/www/html/*'
                sh 'cp img_avatar2.png  /var/www/html'
                sh 'cp index.html  /var/www/html'
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