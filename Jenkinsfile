pipeline {
  agent {
    docker {
      image 'node:8-alpine'
      args '-p 3000:3000'
    }

  }
  stages {
    stage('Install') {
      steps {
        sh 'npm install'
      }
    }
    stage('Test') {
      steps {
        sh 'npm test'
      }
    }
  }
}