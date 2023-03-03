pipeline {
  agent any
  tools {
    nodejs '16.17.0'
  }
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

        stage('Install Libs') {
          steps {
            yarn 'install'
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
}