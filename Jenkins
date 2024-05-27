pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                // Checkout your project from version control (e.g., Git)
                checkout scm
            }
        }
        stage('Build') {
            steps {
                // You can add commands to build your HTML and CSS project here
                sh 'npm install' // Install dependencies if using npm
                sh 'npm run build' // Or any other build command you have
            }
        }
        stage('Test') {
            steps {
                // You can add commands to test your project here
                sh 'npm test' // Or any other test command you have
            }
        }
        stage('Deploy') {
            steps {
                // You can add commands to deploy your project here
                // For example, deploying to a web server
                sh 'npm run deploy' // Or any other deploy command you have
            }
        }
    }
}
