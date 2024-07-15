pipeline {
    agent any
    tools {
        Maven
    }
    stages {
        stage('Build') {
            steps {
                // Build steps, e.g., compile code
                echo 'Building...'
                sh "mvn install"
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