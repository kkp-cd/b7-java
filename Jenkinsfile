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
          bat 'mvn clean'
            }
          }
        stage ('build') {
          steps {
            bat 'mvn clean install'
              }
            }
        }
    }
