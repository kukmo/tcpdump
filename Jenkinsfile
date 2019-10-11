pipeline {
  agent any
  stages {
    stage('Build') {
      agent {
        docker {
          args '-u 0'
          image 'alpine'
        }

      }
      steps {
        sh '''
apk add gcc

'''
        sh 'apk add git'
        sh 'apk add make '
        sh 'apk add libc-dev openssl-dev libpcap-dev'
        sh './configure'
      }
    }
  }
}