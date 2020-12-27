pipeline {
    agent {
        docker { image 'node:8.x' }
    }
    stages {
        stage('Test') {
            steps {
                sh 'node --version'
            }
        }
    }
}
