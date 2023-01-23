pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Building'
      }
    }

    stage('Testing Stage') {
      parallel {
        stage('Testing Stage') {
          steps {
            echo 'Test Number 01'
            sleep 1
            echo 'Test 02'
          }
        }

        stage('Anther Test stage') {
          steps {
            echo 'This is parallel '
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploying'
      }
    }

  }
}