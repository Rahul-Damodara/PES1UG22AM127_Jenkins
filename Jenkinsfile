pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                echo 'Building the application...'
                sh 'make build' // Replace with actual build command
            }
        }
        
        stage('Test') {
            steps {
                echo 'Running tests...'
                sh 'make test' // Replace with actual test command
            }
        }
        
        stage('Deploy') {
            steps {
                echo 'Deploying application...'
                sh 'make deploy' // Replace with actual deploy command
            }
        }
    }
    
    post {
        failure {
            echo 'Pipeline failed'
        }
    }
}

