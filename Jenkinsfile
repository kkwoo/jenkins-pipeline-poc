pipeline {
  agent any
  stages {
    stage('stop') {
      steps {
        powershell(script: 'stop01.ps1', returnStatus: true, returnStdout: true)
      }
    }

    stage('check status') {
      steps {
        powershell(script: 'check-status.ps1', returnStatus: true, returnStdout: true)
      }
    }

  }
}