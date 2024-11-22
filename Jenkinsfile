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
                // Run the .sh script using Git Bash, add --passWithNoTests to allow success even with no tests
                bat '"C:\\Program Files\\Git\\bin\\bash.exe" --login -c "./jenkins/scripts/test.sh" -- --passWithNoTests'
            }
        }
    }
}
