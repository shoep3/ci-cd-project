pipeline {
    agent any
    stages {
        stage('Build Docker image') {
            steps {
                sh 'docker build -t python-app .'
            }
        }
        stage('Test') {
            steps {
                sh 'docker run --rm python-app'
            }
        }
    }
}
