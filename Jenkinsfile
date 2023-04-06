pipeline {
  agent any
  stages {
    stage('pull_code') {
      agent any
      steps {
        sh 'git clone https://github.com/yefen123/job_dsl_gradle_example.git'
      }
    }

    stage('build') {
      steps {
        sh '$PWD/job_dsl_gradle_example/gradlew assemble'
      }
    }

  }
}