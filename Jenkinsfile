pipeline {
  agent {
    docker {
      image 'clojure'
    }

  }
  stages {
    stage('build') {
      steps {
        sh 'echo "Building"'
      }
    }
    stage('Test') {
      steps {
        sh 'lein test'
      }
    }
  }
  post {
    always {
      echo 'Finished'

    }

    success {
      echo 'Successful'

    }

    failure {
      echo 'Failed'

    }

    unstable {
      echo 'Unstable'

    }

  }
}