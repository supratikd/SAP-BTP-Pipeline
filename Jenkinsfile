pipeline {
    agent any
    stages {
       stage('Checkout') {
            steps {
                git 'https://github.com/supratikd/SAP-BTP-Pipeline.git'
            }
        }
        stage('build') {
            steps {
                //sh(script: 'npm install')
            }
        }
    }
}