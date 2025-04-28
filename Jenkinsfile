pipeline {
    agent {
        docker {
            image 'node:18'  // or 'node:20' — pick appropriate version
        }
    }
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
