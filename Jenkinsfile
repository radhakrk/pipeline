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
        build(job: 'pipe-test', propagate: true)
      }
    }
  }
}