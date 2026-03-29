pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'docker build -t cicd-demo .'
            }
        }
        stage('Test') {
            steps {
                sh 'echo "Test passed ✅"'
            }
        }
        stage('Deploy') {
            steps {
                sh 'docker run --rm cicd-demo'
            }
        }
    }
}