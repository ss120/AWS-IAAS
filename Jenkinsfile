pipeline {
  agent any
  stages {
    stage('Source Discovery') {
      steps {
        bat 'python C:\\Python27\\SMS_Jenkins\\Discovery.py'
      }
    }
    stage('Prevalidating Source') {
      steps {
        bat 'call C:\\Python27\\SMS_Jenkins\\prevalidation'
      }
    }
  }
}