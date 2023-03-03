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

        stage('Node Version') {
          steps {
            sh 'node -v'
          }
        }

      }
    }

    stage('Build') {
      steps {
        sh '''npm install -g yarn
yarn install'''
      }
    }

  }
  tools {
    nodejs '16.17.0'
  }
}