pipeline {
    agent any
    tools {
        maven 'Maven' 
    }
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
                sh 'mvn clean install'
            }
        }
        stage('Test') {
            steps {
                // Run tests
                echo 'Testing...'
                sh 'mvn test'
            }
        }
        stage('Deploy') {
            steps {
                // Deploy the application
                echo 'Deploying...'
                // Add your deployment steps here
            }
        }
    }
    post {
        always {
            // Clean up
            echo 'Cleaning up...'
            // Add any necessary cleanup steps here
        }
    }
}
