pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                echo 'Building the application...'
                sh 'nvm install'
            }
        }
        
        stage('Test') {
            steps {
                echo 'Running tests...'
                sh 'npm test'  // Ensure you have tests or modify this step accordingly
            }
        }
        
        stage('Deploy') {
            steps {
                echo 'Deploying the application...'
                // Here you could add deployment steps, like copying files to a server.
            }
        }
    }
}
