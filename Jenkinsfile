pipeline {
  agent {
    node {
      label 'edge'
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