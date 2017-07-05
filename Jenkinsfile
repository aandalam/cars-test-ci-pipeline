pipeline {
  agent any
  stages {
    stage('') {
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