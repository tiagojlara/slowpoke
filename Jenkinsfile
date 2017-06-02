pipeline {
  agent {
    docker {
      image 'node:6.9'
    }
    
  }
  stages {
    stage('build') {
      steps {
        sh 'npm install'
      }
    }
  }
  environment {
    NODE_ENV = 'ci'
  }
}