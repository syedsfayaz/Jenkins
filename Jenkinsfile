pipeline {
  agent any
  environment {
	  XYZ = "XYZ"
	  ZYX = "DIUDH"
  }
  stages {
	  
    stage('Checkout') {
      options { timestamps() }
      parallel {
        stage('pull it') {
          steps {
            echo 'Connecting to git'
            echo 'Doing some thing'
          }
        }
        stage('Pull code') {
          steps {
            echo 'Pull code'
          }
        }
        stage('Store Locally') {
          steps {
            echo 'Store locally'
          }
        }
      }
    }
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'Compiling'
            echo 'Junits'
            echo 'Sonar'
          }
        }
        stage('Compile') {
          steps {
            echo 'Compiling'
          }
        }
      }
    }
    stage('Deploy') {
      parallel {
        stage('Deploy') {
          steps {
            echo 'Install Tc'
            echo 'War file'
            echo 'deploy'
          }
        }
        stage('Deployed to TC') {
          steps {
            echo 'Deployed to TC'
          }
        }
      }
    }
  }
}
