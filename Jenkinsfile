pipeline {
  agent any
  environment {
    NODE_ENV_PATH = './venv'
    NODE_VERSION = '6.11.1'
  }
  stages {
    stage('Build') {
  // Checkout, build
  node {
    checkout scm
    sh 'npm install'
    stash name: 'built'
  }
}
  }
}
