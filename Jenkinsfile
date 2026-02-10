pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                echo 'Building the app...'
                sh 'mvn clean compile -DskipTests'
            }
        }
        
        stage('Test') {
            steps {
                echo 'Running tests...'
                sh 'mvn test'
                junit 'target/surefire-reports/*.xml'
            }
            post {
                always {
                    archiveArtifacts artifacts: 'target/*.jar', allowEmptyArchive: true
                }
            }
        }
        
        stage('Deploy') {
            steps {
                echo 'Deploying to staging...'
                sh 'mvn deploy -DaltDeploymentRepository=staging::default::http://your-nexus:8081/repository/staging/'
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
