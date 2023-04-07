pipeline {
  agent any
  stages {
    stage('pull_code') {
      steps {
        sh 'git clone https://github.com/yefen123/job_dsl_gradle_example.git'
      }
    }

    stage('build') {
      steps {
        sh './job_dsl_gradle_example/gradlew assemble'
      }
    }

    stage('test') {
      steps {
        sh 'echo \'test ...\''
      }
    }

  }
}