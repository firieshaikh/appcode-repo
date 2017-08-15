#!groovy
pipeline {
    
    agent {
        label 'sms-pom-2'
    }
    
    stages {
        stage('Build') {
            steps {
                echo 'Build stage 1: Copying the repo'
                git url "https://github.com/firieshaikh/appcode-repo"
                echo 'Build Stage 2: Deploying docker'
                sh 'docker build -t centos/python-flask .'
                sh 'docker run -d --rm --name python-flask -p 80:80 centos/python-flask'
                
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
