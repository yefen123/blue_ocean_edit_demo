pipeline {
  agent any
  stages {
    stage('pull_code') {
      agent any
      steps {
        sh 'git clone https://github.com/yefen123/job_dsl_gradle_example.git && echo $PWD'
      }
    }

    stage('build') {
      steps {
        sh '/var/jenkins_home/workspace/blue_ocean_edit_demo/job_dsl_gradle_example/gradlew assemble'
      }
    }

  }
}