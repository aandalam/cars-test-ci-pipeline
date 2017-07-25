pipeline {
  agent any
  stages {
    stage('error') {
      steps {
        parallel(
          "Dev": {
            echo 'hello Dev'
            
          },
          "test": {
            sh './deploy.sh'
            
          }
        )
      }
    }
    stage('Test') {
      steps {
        echo 'Hello test env'
      }
    }
  }
}