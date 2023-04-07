pipeline {
  agent any
  stages {
    stage('pull_code') {
      agent any
      steps {
        sh 'echo "clone code .."'
      }
    }

    stage('build') {
      steps {
        sh 'echo \'build ...\''
      }
    }

    stage('test') {
      steps {
        sh 'echo "test ....." > results.xml'
      }
    }

  }
}