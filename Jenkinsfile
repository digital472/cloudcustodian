pipeline {
  agent any
  stages {
    stage('CustodianExecute') {
      steps {
        awsIdentity()
        sh '''
unzip deployment.zip
/usr/local/bin/custodian run --output-dir=. custodian.yml'''
      }
    }
  }
}