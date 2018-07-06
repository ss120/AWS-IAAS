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
    stage('Initiate Migration') {
      steps {
        bat 'python C:\\python27\\SMS_Jenkins\\CreateReplicationJob.py'
      }
    }
    stage('Cutover') {
      steps {
        bat 'python C:\\python27\\SMS_Jenkins\\cutover.py'
      }
    }
    stage('Post Validation') {
      steps {
        bat 'python C:\\python27\\SMS_Jenkins\\post_Migration_Script.py'
      }
    }
  }
}