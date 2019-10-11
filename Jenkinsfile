pipeline {
  agent any
  stages {
    stage('Build') {
      agent {
        docker {
          image 'ubuntu'
          args '-u 0'
        }

      }
      steps {
        sh '''apt update 
apt install gcc

'''
        sh 'apt install git'
        sh 'sudo apt install make'
        sh 'apt install libc-dev openssl-dev make'
        sh './configure && make'
      }
    }
  }
}