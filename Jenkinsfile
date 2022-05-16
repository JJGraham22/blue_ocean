pipeline {
  agent {
    node {
      label 'docker'
    }

  }
  stages {
    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'Testing'
          }
        }

        stage('Parallel') {
          steps {
            echo 'para'
            echo 'Additional'
          }
        }

      }
    }

    stage('Build') {
      steps {
        echo 'Building'
      }
    }

    stage('Clean up') {
      steps {
        echo 'Cleaning'
      }
    }

  }
}