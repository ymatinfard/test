pipeline {
  agent any
  stages {
    stage('Checkout Code') {
      steps {
        git(url: 'https://github.com/ymatinfard/test', branch: 'main')
      }
    }

    stage('/Shell Script') {
      parallel {
        stage('/Shell Script') {
          steps {
            sh 'ls -la'
          }
        }

        stage('Python test') {
          steps {
            sh 'npm i && python python helloworld.py'
          }
        }

      }
    }

  }
}