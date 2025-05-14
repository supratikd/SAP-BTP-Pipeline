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

    stage('Confirm Deploy to staging') {
     steps {
       timeout(time: 60, unit: 'SECONDS') {
         input(message: 'Okay to Deploy?', ok: 'Let\'s Do it!')
       }
     }
   }
    stage('Test') {
      steps {
        echo 'Run tests'
      }
    }
  }
}