pipeline {
  agent {
    node {
      label 'simple-node-project'
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