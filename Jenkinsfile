pipeline {
    agent any
    stages {
        stage('Test') {
            steps {
                sh 'node --version'
                sh 'npm install'
                sh 'npm test'
                // sh 'npm run-script build'
            }
        }
        stage('End Test') {
            steps {
                sh 'echo finished testing'
            }
        }
    }
  
}
