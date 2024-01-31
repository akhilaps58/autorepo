pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                checkout([$class: 'GitSCM', branches: [[name: 'main']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/akhilaps58/autorepo.git']]])
            }
        }

        stage('Build and Deploy') {
            steps {
                // Your build and deploy steps here
            }
        }
    }
}
