pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }
        stage('Build') {
            steps {
                script {
                    sh '''
                        npm install
                    '''
                }
            }
        }
        stage('Test') {
            steps {
                // Test steps here
            }
        }
        stage('Deploy') {
            steps {
                // Deploy steps here
            }
        }
    }
}
