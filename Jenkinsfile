pipeline {
    agent any // Runs on any available build executor

    stages {
        stage('Build') {
            steps {
                echo 'Building application...'
                // For Linux/macOS: sh 'make' or 'mvn clean package'
                // For Windows: bat 'your-build-command'
            }
        }
        stage('Test') {
            steps {
                echo 'Running unit tests...'
                // sh 'npm test' or 'mvn test'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying application...'
            }
        }
    }
    
    post {
        always {
            echo 'Pipeline has completed execution.'
        }
        success {
            echo 'Pipeline succeeded!'
        }
        failure {
            echo 'Pipeline failed. Check logs.'
        }
    }
}
