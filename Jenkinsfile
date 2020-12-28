pipeline {
    agent {
        docker { image 'node:latest' }
    }
    stages {
        stage('Test') {
            steps {
                sh 'node --version'
                sh ' npm install'
                sh 'npm test'
                sh 'npm run-script build'
            }
        }
        stage('End Test') {
            sh 'echo hello world!'
        }
    }
}