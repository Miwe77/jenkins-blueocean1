pipeline {
  agent any
  stages {
    stage('Compile') {
      steps {
        echo 'Estoy compilando'
      }
    }

    stage('Testing') {
      parallel {
        stage('Testing') {
          steps {
            echo 'I am in testing'
          }
        }

        stage('Testing 2') {
          steps {
            sh 'date'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploy'
      }
    }

  }
}