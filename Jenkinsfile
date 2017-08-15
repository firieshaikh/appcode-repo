pipeline {
    
    agent {
        label 'sms-pom-2'
    }
    
    stages {
        stage('Build') {
            steps {
                echo 'Build stage: 1'
                echo 'Build Stage: 2'
            }
        }
        stage('Test') {
            steps {
                echo 'This is Test stage...'
            }
        }
        stage('Deploy') {
            steps {
                echo 'This is Deploy stage...'
            }
        }
    }
    
}
