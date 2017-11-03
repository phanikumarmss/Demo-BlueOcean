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
            sh 'echo welcome2'
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