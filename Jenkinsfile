// test webhook
pipeline {
    agent { docker { image 'node:10.16-alpine' } }
    stages {
        stage('build') {
            steps {
                sh 'pwd'
                sh 'ls'
                sh 'aws --version'
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
