pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            sh 'echo "Building application..."'
          }
        }

        stage('Security') {
          steps {
            sh 'echo "Running parallel security scan..."'
          }
        }

      }
    }

    stage('test') {
      steps {
        sh 'echo "checking the test cases..."'
      }
    }

    stage('deploy') {
      steps {
        sh 'echo "Deploying application..."'
      }
    }

  }
}