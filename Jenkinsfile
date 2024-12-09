pipeline {
    agent any

    tools {
        nodejs "NodeJS_LTS"
    }

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Install') {
            steps {
                sh 'npm install'
            }
        }

        stage('Build') {
            steps {
                sh 'node app.js'
            }
        }

        stage('Deploy') {
            steps {
                echo "Deployment complete."
            }
        }
    }
}
