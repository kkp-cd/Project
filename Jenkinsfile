pipeline {
  agent {label 'linux_kiran'}
    stages {
      stage ('pull') {
        steps {
        git branch:'main', url:'https://github.com/kkp-cd/Project.git'
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
