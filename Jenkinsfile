pipeline {
  agent any
  stages {
    stage('CustodianExecute') {
      steps {
        awsIdentity()
        sh '''
/usr/local/bin/custodian run --output-dir=. custodian.yml'''
      }
    }
  }
}