pipeline {
  agent any
  stages {
    stage('Build Assets') {
      steps {
        echo 'Building Assets'
      }
    }
    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'Testing some stuff ////'
          }
        }
        stage('New Stage') {
          steps {
            bat(returnStatus: true, returnStdout: true, label: 'haha', script: 'dir C:\\')
          }
        }
      }
    }
  }
}