pipeline {
    agent {
        docker { image 'node:latest' }
    }
    stages {
        stage('Test') {
            steps {
                sh 'node --version'
                sh 'npm cache clean --force'
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