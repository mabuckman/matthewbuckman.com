// test webhook
pipeline {
    agent { dockerfile true }
    stages {
        stage('build') {
            steps {
                sh 'aws --version'
                sh 'node --version'
                sh 'npm install'
                sh 'ng build'
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
