pipeline {
  agent any
  stages {
    stage('Dev') {
      steps {
        echo 'This is development stage'
      }
    }

    stage('Buid') {
      steps {
        echo 'This is build stage'
      }
    }

    stage('Test') {
      steps {
        echo 'This is test stage'
      }
    }

    stage('UAT') {
      parallel {
        stage('UAT') {
          steps {
            echo 'UAT stage'
          }
        }

        stage('Deploye') {
          steps {
            echo 'deploye stage'
          }
        }

        stage('operate stage') {
          steps {
            echo 'this is operate stage'
          }
        }

      }
    }

  }
}