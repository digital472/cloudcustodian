pipeline {
  agent any
  stages {
    stage('CustodianExecute') {
      steps {
        sh 'custodian custodian run --output-dir=. /home/ec2-user/custodian.yml'
      }
    }
  }
}