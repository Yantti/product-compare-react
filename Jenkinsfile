pipeline {
  agent any
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