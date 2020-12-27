pipeline {
  
    agent any
    stages {
        stage('front & back') {
          matrix{
            axes {
              axis{
                name: 'node-version'
                values: '8.x"
              }
            }
          }
          agent{
            label "${node-version}"
          }
          stages{
            stage('front'){nodejs "8.x"}
            steps {
                echo 'Hello World'
            }
          }
        }
    }
}
