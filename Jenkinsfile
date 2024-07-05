pipeline {
    agent any
    stages {
        stage('Clone') {
            steps {
                // Clone repository từ GitHub
                git 'https://github.com/nguyenthai-duong/test_jenkins2.git'
            }
        }
        stage('Build') {
            steps {
                // Chạy script build
                sh './build.sh'
            }
        }
        stage('Test') {
            steps {
                // Chạy script test
                sh './test.sh'
            }
        }
        stage('Deploy') {
            steps {
                // Chạy script deploy
                sh './deploy.sh'
            }
        }
    }
}
