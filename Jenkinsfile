// pipeline {
//     agent any
//     stages {
//        stage('Checkout') {
//             steps {
//                 git 'https://github.com/supratikd/SAP-BTP-Pipeline.git'
//             }
//         }
//         stage('build') {
//             steps {
//                 sh 'npm install' 
//             }
//         }
//     }
// }


pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        bat 'npm install' 
      }
    }
    stage('Test') {
      steps {
        echo 'Run tests'
      }
    }
  }
}