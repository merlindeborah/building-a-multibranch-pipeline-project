pipeline {
    agent any
    environment {
        CI = 'true'
    }
    stages {
        stage('Build') {
            steps {
                bat 'npm install'
            }
        }
        stage('Test') {
            steps {
                // Call the .sh script using Git Bash
                bat './jenkins/scripts/test.bat'
            }
        }
    }
}
