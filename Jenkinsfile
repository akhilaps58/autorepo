pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                script {
                    // Clean workspace before checkout
                    deleteDir()

                    // Clone the repository without specifying a refspec
                    checkout([$class: 'GitSCM', userRemoteConfigs: [[url: 'https://github.com/akhilaps58/autorepo.git']]])
                }
            }
        }

        stage('Build and Deploy') {
            steps {
                // Your build and deploy steps here
                echo 'Build and deploy steps go here'
            }
        }
    }
}
