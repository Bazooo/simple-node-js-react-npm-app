pipeline {
  agent {
    node {
      label 'test'
    }
    
  }
  stages {
    stage('Build') {
      steps {
        sh 'npm install'
      }
    }
  }
}