pipeline {
  agent any
  stages {
    stage('plan') {
      steps {
        echo 'This is plan stage'
      }
    }

    stage('code') {
      steps {
        echo 'this is code stage'
      }
    }

    stage('build') {
      steps {
        echo 'this is build stage'
      }
    }

    stage('Test') {
      steps {
        echo 'this is test stage'
      }
    }

    stage('Release') {
      steps {
        echo 'this is release stage'
      }
    }

    stage('Deploy') {
      parallel {
        stage('Deploy') {
          steps {
            echo 'this is deploy stage'
          }
        }

        stage('operate') {
          steps {
            echo 'this is operate stage'
          }
        }

      }
    }

  }
}