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
            echo '"Testing"'
          }
        }

        stage('Parallel') {
          steps {
            echo '"running an enviroment in pipeline"'
          }
        }

      }
    }

    stage('Build') {
      steps {
        echo '"building environment"'
      }
    }

    stage('Final') {
      steps {
        echo '"clean up"'
      }
    }

  }
}