pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'build comoleted'
      }
    }

    stage('Test stages') {
      parallel {
        stage('Test2') {
          steps {
            echo 'running test2'
          }
        }

        stage('Test 1') {
          steps {
            echo 'runnung Test1 '
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'running deploy'
      }
    }

  }
}