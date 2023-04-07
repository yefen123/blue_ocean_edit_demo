pipeline {
  agent any
  stages {
    stage('pull') {
      steps {
        sh 'echo \'clone code ..\' '
      }
    }

    stage('build') {
      steps {
        sh 'echo \'build ...\''
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            sh 'echo \'test\''
          }
        }

        stage('test2') {
          steps {
            sh 'echo \'test2\''
          }
        }

      }
    }

  }
}