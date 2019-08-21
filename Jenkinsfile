pipeline {
  agent any
  stages {
    stage('build') {
      parallel {
        stage('build') {
          steps {
            input message: 'Finished using the web site? (Click "Proceed" to continue)'
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
        sh 'echo "done"'
      }
    }
  }
}