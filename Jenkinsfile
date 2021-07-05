pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'This is stage1'
            sleep 2
          }
        }

        stage('Static Code Analysis') {
          steps {
            echo 'running static code analysis'
          }
        }

      }
    }

    stage('Unit tests') {
      steps {
        echo 'Running unit tests'
      }
    }

    stage('Automated tests') {
      steps {
        sleep 2
      }
    }

    stage('Publish the Artifacts') {
      steps {
        echo 'publishing'
      }
    }

    stage('Email Notification') {
      steps {
        echo 'Sending email'
      }
    }

  }
}