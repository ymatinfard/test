pipeline {
  agent any
  stages {
    stage('Checkout Code') {
      steps {
        git(url: 'https://github.com/ymatinfard/test', branch: 'main')
      }
    }

    stage('/Shell Script') {
      steps {
        sh '''sh \'python helloworld.py\'
       '''
      }
    }

  }
}