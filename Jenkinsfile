pipeline {
  agent any
  stages {
    stage('checkout code') {
      steps {
        git(url: 'https://github.com/annfii/juice-shop', branch: 'master')
      }
    }

    stage('install & test') {
      steps {
        sh 'npm install && npm test'
      }
    }

  }
}