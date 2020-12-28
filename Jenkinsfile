pipeline {
    agent any
    stages {
        stage('Test') {
            steps {
                sh 'node --version'
                sh 'npm install'
                sh 'npm test'
                // sh 'npm run-script build'
                sh 'echo 1'
            }
        }
        stage('Docker build back images') {
            steps {
                sh 'docker build -t nhadjarab/back-devops-project:latest -f Dockerfile.back .'
            }
        }
        stage('Docker build front images') {
            steps {
                sh 'docker build -t nhadjarab/front-devops-project:latest -f Dockerfile.front .'
            }
        }
    }
  
}
