pipeline {
  agent none
  stages {
    stage('unit') {
      agent any
      environment {
        PATH = 'C:\\Program Files\\Maven\\apache-maven-3.6.0\\bin'
      }
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