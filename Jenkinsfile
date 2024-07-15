pipeline {
	agent any
	tools {
	    Maven
	}
	stages {
		stage("checkout") {
			steps {
			    echo 'Checking out the application...'
			}
		}
		stage("build") {
			steps {
			    sh "mvn install"
			}
		}
		stage("test") {
            steps {
                echo 'testing the application...'
            }
        }
		stage("deploy") {
            steps {
                echo 'deploying the application...'
            }
        }
	}
}