pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'g++ -o task5 main/task5.cpp'
        echo 'Build Successful!'
      }
    }
    stage('Test') {
      steps {
        sh './task5'
        echo 'Test Successful!'
      }
    }
    stag('Deploy') {
      steps {
        echo 'Successfully deployed!'
      }
    }
  }
  post {
    failure {
      echo 'Pipeline Failed!'
    }
  }
}
