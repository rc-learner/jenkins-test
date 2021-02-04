#!/usr/bin/groovy

pipeline {
  agent any

  stages {
    stage('Checkout') {
      steps {
        checkout scm
      }
    }
    stage('Unit Testing'){
      steps {
        script {
          sh pytest test_mypython.py
        }
      }
    }
  }
}
