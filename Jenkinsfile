pipeline {
  agent any
  stages {
    stage('CustodianExecute') {
      steps {
        sh '''pwd
/usr/local/bin/custodian run --output-dir=. /home/ec2-user/custodian.yml'''
      }
    }
  }
}