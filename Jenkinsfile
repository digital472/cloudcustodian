pipeline {
  agent any
  stages {
    stage('CustodianExecute') {
      steps {
        sh '/usr/local/bin/custodian run --output-dir=. /home/ec2-user/custodian.yml'
      }
    }
  }
}