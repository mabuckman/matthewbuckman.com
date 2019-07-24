// test webhook
pipeline {
    agent { dockerfile true }
    environment {
        HOME = '.'
        npm_config_cache = 'npm-cache'
    }
    stages {
        stage('build') {
            steps {
                sh 'npm -g install'
                sh 'ng build'
                sh 'ls'
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
