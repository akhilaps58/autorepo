pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Build and Deploy') {
            steps {
                // You can add build and deploy commands here
                // For simplicity, let's say you are copying files to your web server's directory
                sh 'cp -r * /var/www/html/'
            }
        }
    }
}
