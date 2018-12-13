pipeline {
  agent any
  stages {
    stage('CustodianExecute') {
      steps {
        sh '''pip install c7n
custodian run --output-dir=. /home/ec2-user/custodian.yml'''
      }
    }
  }
}