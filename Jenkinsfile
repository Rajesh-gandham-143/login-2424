pipeline {
    agent any 
    stages{
        stage('deploy') {
            steps{
                sh 'rm -rf /var/www/html/*'
                sh 'cp . /var/www/html'
            }

        }
    }
    
}