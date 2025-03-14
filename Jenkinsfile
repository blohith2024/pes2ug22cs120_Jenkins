pipeline {
    agent any  // This runs on any available agent

    stages {
        stage('Clone Repository') {
            steps {
                git branch: 'main', url: 'https://github.com/blohith2024/pes2ug22cs120_Jenkins.git'
            }
        }

        stage('Build') {
            steps {
                echo 'Building the project...'
                sh 'echo Build successful'  // Replace with actual build command
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                sh 'echo Tests passed'  // Replace with actual test command
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application...'
                sh 'echo Deployment complete'  // Replace with actual deployment command
            }
        }
    }

    post {
        success {
            echo 'Pipeline executed successfully!'
        }
        failure {
            echo 'Pipeline failed!'
        }
    }
}
