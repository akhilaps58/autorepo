pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                script {
                    // Clean workspace before checkout
                    deleteDir()

                    // Clone the repository and specify the branch
                    checkout([$class: 'GitSCM', branches: [[name: 'master']], userRemoteConfigs: [[url: 'https://github.com/akhilaps58/autorepo.git']]])
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
