pipeline {
  agent any
  stages {
    stage('docker example') {
      parallel {
        stage('docker example') {
          steps {
            sh 'java --version'
          }
        }

        stage('python') {
          steps {
            sh 'python --version'
          }
        }

      }
    }

    stage('success') {
      steps {
        echo 'good day'
      }
    }

  }
}