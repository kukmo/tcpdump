pipeline {
  agent any
  stages {
    stage('Build') {
      agent {
        docker {
          image 'ubuntu'
        }

      }
      steps {
        sh '''
apt install gcc

'''
        sh 'apt install git'
        sh 'sudo apt install make'
        sh 'apt install libc-dev openssl-dev make'
      }
    }
  }
}