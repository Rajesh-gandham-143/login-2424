pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'sudo rm -rf /var/www/html/*'
                sh 'sudo cp -r img_avatar2.png /var/www/html/'
                sh 'sudo cp -r index.html /var/www/html/'
            }
        }
        stage('Test') {
            steps {
                sh 'sudo docker run  --rm -e SONAR_HOST_URL="http://localhost:9000" -e SONAR_LOGIN=" sqp_5adb081b55bf930d65029d99b1b8d63d35e33bb5"  -v ".:/usr/src" sonarsource/sonar-scanner-cli:5.0 -Dsonar.projectKey=login-2424'
            }
        }
        stage('Deploy') {
            steps {
                sh 'free '
            }
        }
    }
}