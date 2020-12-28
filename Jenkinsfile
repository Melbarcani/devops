pipeline {
    agent {
        docker { image 'node:latest' }
    }
    stages {
        stage('Test') {
            steps {
                sh 'node --version'
                sh 'chown -R 111:115 "/.npm"'
                sh ' npm install'
                sh 'npm test'
                sh 'npm run-script build'
            }
        }
        stage('End Test') {
            steps {
                sh 'echo hello world!'
            }
        }
    }
}