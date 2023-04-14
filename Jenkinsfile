pipeline {
  agent {
    node {
      label 'docker'
    }

  }
  stages {
    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'test'
          }
        }

        stage('Parrallel') {
          steps {
            echo 'message'
          }
        }

      }
    }

    stage('Build') {
      steps {
        build 'building'
      }
    }

    stage('clean up ') {
      steps {
        echo 'cleaning '
      }
    }

  }
  environment {
    Name = 'Value'
  }
}