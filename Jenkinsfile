pipeline {
  agent any
  stages {
    stage('Checkout') {
      steps {
        echo 'Connecting to git'
        echo 'Pulling Code'
        echo 'Doing some thing'
      }
    }
    stage('Build') {
      steps {
        echo 'Compiling'
        echo 'Junits'
        echo 'Sonar'
      }
    }
    stage('Deploy') {
      steps {
        echo 'Install Tc'
        echo 'War file'
        echo 'deploy'
      }
    }
  }
}