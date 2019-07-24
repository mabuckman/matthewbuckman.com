// test webhook
pipeline {
    agent { docker { image 'node:10.16-alpine' } }
    stages {
        stage('build') {
            steps {
                sh 'npm i'
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
