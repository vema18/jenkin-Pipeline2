pipeline {
  agent any
  stages {
    stage('plane') {
      steps {
        echo 'I want to plane my application developement'
      }
    }

    stage('code') {
      steps {
        echo 'deveplement team start working on the application'
      }
    }

    stage('build') {
      steps {
        echo 'build the application'
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'test team perform activity'
          }
        }

        stage('deploy') {
          steps {
            echo 'deploy the war files'
          }
        }

        stage('release') {
          steps {
            echo 'move to release '
          }
        }

        stage('operate') {
          steps {
            echo 'test application'
          }
        }

      }
    }

  }
}