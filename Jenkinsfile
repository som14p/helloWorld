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
        stage('firefox') {
          steps {
            echo 'Test stp no 1'
          }
        }
        stage('chrome') {
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
  }
}