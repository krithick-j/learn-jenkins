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
                        export NVM_DIR="$HOME/.nvm"
                        [ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh" # Load nvm
                        nvm install 14 # This installs Node.js 14 and uses it
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
