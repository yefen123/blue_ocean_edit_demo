pipeline {
  agent any
  stages {
    stage('pull_code') {
      steps {
        sh '''echo \'clone code\'
echo \'clone code2\''''
        git 'https://github.com/yefen123/job_dsl_gradle_example.git'
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
  post {
    always {
      sh 'echo $COMPLETED_MSG'
    }

  }
}