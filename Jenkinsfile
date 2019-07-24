// test webhook
pipeline {
    agent { dockerfile true }
    stages {
        stage('build') {
            steps {
                sh 'aws --version'
                sh 'node --version'
                sh 'ng build'
                sh 'npm install'
            }   
        }
        stage('deploy') {
            steps {
                sh 'pwd'
                sh 'aws --version'
            }   
        }
    }
} 
