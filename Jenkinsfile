pipeline {
    agent any
   // {        docker { image 'node:18' }     }
    stages {
        stage('Clone') {
            steps {
                git 'https://github.com/YOUR_USERNAME/jenkins-demo.git'
            }
        }
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
                sh 'node index.js'
            }
        }
    }
}
