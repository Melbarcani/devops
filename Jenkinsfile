pipeline {
    agent {
        docker { image 'node:14-alpine' }
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
    }
}