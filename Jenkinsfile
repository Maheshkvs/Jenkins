pipeline {
  agent any
  stages {
    stage('Stage 1') {
      parallel {
        stage('Stage 1') {
          steps {
            echo 'Hello PipeLine 1'
          }
        }
        stage('Stage 1 -2') {
          steps {
            build(job: 'example-maven-project', quietPeriod: 2)
          }
        }
      }
    }
    stage('Blue stage') {
      steps {
        sleep 1
      }
    }
  }
}