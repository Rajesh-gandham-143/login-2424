pipeline {
    agent any 
    stages{
        stage('deploy') {
            steps{
                sh 'rm -rf /var/www/html/*'
                sh 'copy . /var/www/html'
            }

        }
    }
    
}