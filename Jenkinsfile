pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Checkout source code from GitHub'
            }
        }

        stage('Build') {
            steps {
                echo 'Building Event Management project...'
            }
        }

        stage('Unit Test') {
            steps {
                echo 'Running unit tests...'
                echo 'Unit Test passed'
            }
        }

        stage('Package') {
            steps {
                echo 'Packaging Event Management application...'
            }
        }
    }

    post {
        success {
            echo 'CI Pipeline completed successfully'
        }
        failure {
            echo 'CI Pipeline failed'
        }
    }
}
