pipeline {
    agent any
    environment {
        CI = 'true'
    }
    stages {
        stage('Build') {
            steps {
                // Install dependencies using npm
                bat 'npm install'
            }
        }
        stage('Test') {
            steps {
                // Use a batch file instead of a shell script for Windows
                bat 'jenkins\\scripts\\test.bat'
            }
        }
    }
}
