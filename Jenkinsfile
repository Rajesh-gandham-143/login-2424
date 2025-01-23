pipeline {
    agent any 
    stages{
        stage('deploy') {
            steps{
                sh 'sudo rm -rf /var/www/html/*'
                sh 'sudo copy . /var/www/html'
            }

        }
    }
    
}