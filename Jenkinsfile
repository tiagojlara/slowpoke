pipeline {
  agent {
    docker {
      image 'node:6.9'
    }
    
  }
  stages {
    stage('build') {
      steps {
        parallel(
          "build": {
            sh 'npm install'
            
          },
          "test": {
            sh 'npm -v'
            
          }
        )
      }
    }
  }
  environment {
    NODE_ENV = 'ci'
  }
}