pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh '''echo "hi"
pwd'''
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'test step'
          }
        }

        stage('test para') {
          steps {
            echo 'parallel step'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'delpoy massage'
      }
    }

  }
}