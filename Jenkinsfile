pipeline {
    agent any

    stages {

        stage('Install Dependencies') {
            steps {
                sh 'npm install'
            }
        }

        stage('Build') {
            steps {
                sh 'node --check src/app.js'
            }
        }

        stage('Test') {
            steps {
                sh 'npm test'
            }
        }
    }
}
