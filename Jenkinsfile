pipeline {
  agent none
  stages {
    stage('unit') {
      steps {
        sh 'mvn clean test'
      }
    }
    stage('integtaion test') {
      steps {
        sh 'echo \'Integration\''
      }
    }
    stage('UI test') {
      steps {
        build 'Smoke_UI_Test'
      }
    }
  }
}