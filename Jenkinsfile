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
    stage('Deliver') {
      steps {
        sh './jenkins/scripts/deliver.sh'
        input(message: 'Finished using the web site? (Click "Proceed" to continue)', ok: 'Proceed')
        sh './jenkins/scripts/kill.sh'
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