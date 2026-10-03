pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                echo 'Building the application...'
                bat 'npm install'
            }
        }

        // Jenkins CI/CD Task 2

        stage('Test') {
            steps {
                echo 'Running tests...'
                bat 'npm test'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying the application...'
                bat 'echo Application deployed successfully!'
            }
        }
    }
}
