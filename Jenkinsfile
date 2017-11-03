pipeline {
  agent any
  stages {
    stage('BuildGroup') {
      parallel {
        stage('error') {
          steps {
            sh 'echo welcome'
          }
        }
        stage('build2') {
          steps {
            sh 'echo papajohns'
            sleep 10
            retry(count: 10)
          }
        }
      }
    }
    stage('error') {
      steps {
        sh 'echo welcome end'
      }
    }
  }
}