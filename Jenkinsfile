pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                // Checkout code from version control
                git 'https://github.com/Nimish1712/test-project.git'
            }
        }
        stage('Build') {
            steps {
                // Build steps, e.g., compile code
                echo 'Building...'
            }
        }
        stage('Test') {
            steps {
                // Run tests
                echo 'Testing...'
            }
        }
        stage('Deploy') {
            steps {
                // Deploy the application
                echo 'Deploying...'
            }
        }
    }
    post {
        always {
            // Clean up
            echo 'Cleaning up...'
        }
    }
}
