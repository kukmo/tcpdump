pipeline {
  agent any
  stages {
    stage('Build') {
      agent {
        docker {
          image 'alpine'
        }

      }
      steps {
        sh '''whoami
apk add gcc
./configure
'''
      }
    }
  }
}