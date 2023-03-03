pipeline {
  agent any
  stages {
    stage('Checkout Code') {
      steps {
        git(url: 'https://github.com/mbriceno/portfolio.git', branch: 'main')
      }
    }

    stage('Log') {
      parallel {
        stage('Log') {
          steps {
            sh 'ls -all'
          }
        }

        stage('') {
          steps {
            sh 'node -v'
          }
        }

      }
    }

    stage('Build') {
      steps {
        sh 'node --version'
      }
    }

  }
  tools {
    nodejs '16.17.0'
  }
}