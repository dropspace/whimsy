pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'ls -lh'
      }
    }
    stage('Browser Tests') {
      steps {
        parallel(
          "Firefox": {
            sh 'echo \'setting up selenium environment\''
            
          },
          "Safari": {
            sh 'echo \'setting up selenium environment\''
            
          },
          "Chrome": {
            sh 'echo \'setting up selenium environment\''
            
          },
          "Internet Explorer": {
            sh 'echo \'setting up selenium environment\''
            
          }
        )
      }
    }
    stage('Static Analysis') {
      steps {
        sh 'ls -l'
      }
    }
    stage('Deploy') {
      steps {
        sh 'ls -lh'
      }
    }
  }
  environment {
    DEBUG = 'true'
  }
}