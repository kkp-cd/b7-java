pipeline {
  agent {label 'windows_slave_kiran'}
    stages {
      stage ('pull') {
        steps {
        git branch:'main', url:'https://github.com/kkp-cd/b7-java.git'
        }
      }
      stage ('clean') {
        steps {
          sh 'mvn clean'
            }
          }
        stage ('build') {
          steps {
            sh 'mvn clean install'
              }
            }
        }
    }
