pipeline {
  agent any
  stages {
    stage('Checkout Code') {
      steps {
        git(url: 'https://github.com/mbriceno/portfolio.git', branch: 'main')
      }
    }

    stage('') {
      steps {
        sh 'ls -all'
      }
    }

  }
}