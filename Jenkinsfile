pipeline {
  agent none
  stages {
    stage('build') {
      parallel {
        stage('linux-armv6') {
          agent {label 'Tomcat server slave'}
          steps {
            sh 'echo linux-armv6'
          }
        }
        stage('darwin-amd64') {
          agent {label 'Tomcat server slave'}
          steps {
            sh 'echo darwin-amd64'
          }
        }
        stage('linux-amd64') {
          agent {label 'Tomcat server slave'}
          steps {
            sh 'echo linux-amd64'
          }
        }
      }
    }
  }
}
