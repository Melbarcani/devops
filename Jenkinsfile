pipeline {
    agent {
        docker { image 'node:8' }
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
