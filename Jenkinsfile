pipeline {
    agent {
        docker { image 'clojure' }
    }
    stages {
        stage('build') {
            steps {
                sh 'echo "Building"'
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
