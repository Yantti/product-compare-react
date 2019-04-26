pipeline {
  agent {
    docker {
      image 'node:8-alpine'
      args '-p 3000:3000'
    }

  }
  stages {
    stage('Docker image') {
      steps {
        sh 'docker build -t demo .'
      }
    }
    stage('Run Docker') {
      steps {
        sh 'docker run -t -p 3000:3000 demo'
      }
    }
  }
}