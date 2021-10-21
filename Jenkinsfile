pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'log '
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            sh '''echo "test running"
'''
          }
        }

        stage('test1') {
          steps {
            echo 'anything '
          }
        }

      }
    }

    stage('Deploy ') {
      steps {
        sh 'sh "bash /build"'
      }
    }

  }
}