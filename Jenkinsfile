pipeline {
  agent any
  stages {
    stage('Checkout Code') {
      steps {
        git(url: 'https://github.com/mbriceno/portfolio.git', branch: 'main')
      }
    }

    stage('Log') {
      steps {
        sh 'ls -all'
      }
    }

  }
}