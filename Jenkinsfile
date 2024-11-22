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
                // Correctly call the .bat file
                bat 'jenkins\\scripts\\test.bat'
            }
        }
    }
}
