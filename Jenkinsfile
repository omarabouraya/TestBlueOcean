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
        input(message: 'are you sure u want deploy', ok: 'yes im sure')
        echo 'mission completed'
      }
    }

    stage('notify for new built') {
      steps {
        echo 'new built completed successfully'
      }
    }

  }
}