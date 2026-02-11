pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                echo 'Building the app...' 
                echo 'build completed' 
          }
        }
        
        stage('Test') {
            steps {
                echo 'Running tests...'
                echo 'testing completed'
            }
        }
        
        stage('Deploy') {
            steps {
                echo 'Deploying to staging...'
                echo 'deploying completed'
            }
        }
    }
    
    post {
        success {
            echo 'rizwana successfully depolyed a ci cd pipeline!'
        }
        failure {
            echo 'oops!i messed pipeline'
        }
    }
}
