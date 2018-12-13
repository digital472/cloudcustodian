pipeline {
  agent any
  stages {
    stage('CustodianExecute') {
      steps {
        sh '''virtualenv --python=/usr/bin/python custodian
source custodian/bin/activate
pip install c7n
custodian run --output-dir=. /home/ec2-user/custodian.yml'''
      }
    }
  }
}