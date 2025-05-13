pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/supratikd/SAP-BTP-Pipeline.git'
            }
        }
        // stage('Build') {
        //     steps {
        //         script {
        //             sh 'npm install' // Or yarn install, depending on your project
        //             sh 'ng build --prod' // Build for production
        //             // Run tests here if needed: sh 'ng test'
        //         }
        //     }
        // }
        // stage('Deploy') {
        //     when {
        //         anyOf {
        //             branch "master"
        //             branch "main" // Or your main branch
        //         }
        //     }
        //     steps {
        //         script {
        //             // Implement deployment steps based on your environment (e.g., AWS S3, remote server)
        //             // Example for deploying to AWS S3:
        //             // aws s3 sync dist/YOUR_PROJECT_NAME s3://YOUR_BUCKET_NAME --delete
        //         }
        //     }
        // }
    }
}