pipeline {
    agent any
    tools {
        maven 'Maven' // Ensure Maven tool is configured in Jenkins
        git 'Git'     // Ensure Git tool is configured in Jenkins
    }
    stages {
        stage('Checkout') {
            steps {
                // Checkout code from version control
                echo 'Checking out...'
                //git credentialsId: 'c7447bee-5339-4f33-ae27-42e10189ccba', url: 'https://github.com/Nimish1712/test-project'
            }
        }
        stage('Build') {
            steps {
                // Build steps, e.g., compile code
                echo 'Building...'
                bat 'mvn clean install'
            }
        }
        stage('Test') {
            steps {
                // Run tests
                echo 'Testing...'
                bat 'mvn test'
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
