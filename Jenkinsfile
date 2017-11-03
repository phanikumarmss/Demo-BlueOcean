pipeline {
  agent any
  stages {
    stage('BuildGroup') {
      parallel {
        stage('') {
          steps {
            sh 'echo welcome'
          }
        }
        stage('build2') {
          steps {
            sh 'echo welcome2'
            retry(count: 3)
          }
        }
      }
    }
    stage('') {
      steps {
        sh 'echo welcome end'
      }
    }
  }
}