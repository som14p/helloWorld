pipeline {
  agent any
  stages {
    stage('Initialise') {
      steps {
        echo 'This is first step for Initialize stage'
        sh 'echo initialise'
      }
    }
    stage('Build') {
      steps {
        echo 'Code is getting built and configure'
      }
    }
    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'Test stp no 1'
          }
        }
        stage('test') {
          steps {
            echo 'test no 2'
          }
        }
      }
    }
    stage('Report') {
      steps {
        echo 'This is report'
      }
    }
    stage('End') {
      steps {
        echo 'this is the end of pipeline'
      }
    }
  }
}