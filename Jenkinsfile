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
                // Use 'sh' step to call Git Bash and run the .sh script
                bat '"C:\\Program Files\\Git\\bin\\bash.exe" ./jenkins/scripts/test.sh'
            }
        }
    }
}
