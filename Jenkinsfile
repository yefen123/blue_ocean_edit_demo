pipeline {
  agent any
  stages {
    stage('pull_code') {
      steps {
        sh 'echo \'clone code\''
      }
    }

    stage('build') {
      steps {
        sh 'echo \'building\''
      }
    }

    stage('deploy') {
      parallel {
        stage('deploy') {
          steps {
            sh 'echo \'deploy...\''
          }
        }

        stage('test') {
          steps {
            sh 'echo \'test\''
          }
        }

      }
    }

  }
  environment {
    COMPLETED_MSG = 'build done'
  }
}