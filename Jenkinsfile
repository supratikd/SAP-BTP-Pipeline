pipeline {
  agent any
  stages {
    stage('Checkout') {
        steps {
          git 'https://github.com/supratikd/SAP-BTP-Pipeline.git'
        }
    }
    stage('Build') {
      steps {
        bat 'npm install' 
        bat 'npm run ng -- build' 
      }
    }
    stage('Test') {
      steps {
        echo 'Run tests'
      }
    }
  }
}