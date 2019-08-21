pipeline {
  agent any
  stages {
    stage('build') {
      parallel {
        stage('build') {
          steps {
            sh 'echo "build"'
          }
        }
        stage('push') {
          steps {
            sh 'echo "push"'
          }
        }
        stage('deploy') {
          steps {
            sh 'ls'
          }
        }
      }
    }
    stage('done') {
      steps {
        sh '''echo
    "done"'''
      }
    }
  }
}