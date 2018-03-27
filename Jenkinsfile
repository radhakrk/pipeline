pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'hello pipeline'
      }
    }
    stage('Compile') {
      steps {
        build 'pipe-test'
      }
    }
  }
}