pipeline {
  agent {
    node {
      label 'build'
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