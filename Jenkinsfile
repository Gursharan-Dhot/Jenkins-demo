pipeline {
    agent any

    stages {
        stage('Install Dependencies') {
            steps {
                sh 'npm install'
            }
        }
        stage('Run Test') {
            steps {
                sh 'npm test'
            }
        }
        stage('Run App') {
            steps {
                sh 'npm start'
            }
        }
    }
}
