pipeline {
  agent any
  stages {
    stage('test') {
      steps {
        echo 'for testing code'
      }
    }

    stage('build') {
      steps {
        echo 'build latest code'
      }
    }

    stage('deploy') {
      steps {
        echo 'latest code has been pre deploy mode '
      }
    }

    stage('manual test') {
      steps {
        retry(count: 3)
        sleep 10
      }
    }

    stage('wireup') {
      steps {
        retry(count: 2)
      }
    }

    stage('commit') {
      steps {
        sleep 10
      }
    }

  }
}