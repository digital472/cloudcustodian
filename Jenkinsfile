pipeline {
  agent any
  stages {
    stage('CustodianExecute') {
      steps {
        awsIdentity()
        sh '''
unzip deployment.zip
/usr/local/bin/custodian run --output-dir=. my-first-policy.yml --region us-gov-west-1'''
      }
    }
  }
}