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
                echo 'Building the project...'
                // Add build commands here, e.g., compile, npm build, etc.
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests...'
                // Add test commands here, e.g., ./run-tests.sh or pytest, etc.
            }
        }
    }
    post {
        success {
            echo 'Build and tests succeeded!'
        }
        failure {
            echo 'Build or tests failed.'
        }
    }
}
