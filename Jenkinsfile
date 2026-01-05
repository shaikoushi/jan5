pipeline {
    agent any

    stages {
        stage('Checkout Code') {
            steps {
                echo "Checking out source code..."
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo "Build stage started"
                sh 'echo Build successful'
            }
        }

        stage('Test') {
            steps {
                echo "Test stage started"
                sh 'echo Tests passed'
            }
        }

        stage('Deploy') {
            steps {
                echo "Deploy stage started"
                sh 'echo Deployment completed'
            }
        }
    }

    post {
        success {
            echo "Pipeline executed successfully 🎉"
        }
        failure {
            echo "Pipeline failed ❌"
        }
    }
}
