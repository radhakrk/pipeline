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
    stage('MSBuild') {
      steps {
        bat 'C:\\Users\\sxanandv\\Desktop\\MSBUILD\\Batch-files\\MSBUILD.bat'
      }
    }
    stage('') {
      steps {
        bat(script: 'Unzip.bat', returnStatus: true, returnStdout: true)
      }
    }
  }
}