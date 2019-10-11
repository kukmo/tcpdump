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
        sh '''
apt install gcc

'''
        sh 'sudo apk add sudo'
        sh 'sudo apt install make'
        sh 'apt install libc-dev openssl-dev make'
      }
    }
  }
}