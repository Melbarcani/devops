pipeline {
    agent {
        docker { image 'node:8-alpine3.10' }
    }
    stages {
        stage('Test') {
            steps {
                sh 'npm install'
              sh 'npm test'
            }
        }
    }
}
