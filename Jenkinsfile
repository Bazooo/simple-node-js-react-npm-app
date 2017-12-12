pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'npm install'
      }
    }
    stage('Test') {
      steps {
        sh './jenkins/scripts/test.sh'
      }
    }
  }
  tools {
    nodejs 'edge'
  }
  environment {
    CI = 'true'
  }
}