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
                // Use 'bat' step to run Git Bash to execute the .sh script
                bat '"C:\\Program Files\\Git\\bin\\bash.exe" -c "./jenkins/scripts/test.sh"'
            }
        }
    }
}
