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
                sh 'npm install'
                sh './node_modules/@angular/cli/bin/ng build --prod'
            }   
        }
        stage('deploy') {
            steps {
                sh 'aws s3 cp ./dist/matthewbuckman s3://www.matthewbuckman.com --acl public-read --recursive' 
            }   
        }
    }
} 
