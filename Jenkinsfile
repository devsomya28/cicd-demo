pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'npm install'
            }
        }

        stage('Test') {
            steps {
                sh 'echo "No tests yet"'
            }
        }

        stage('Docker Build') {
            steps {
                sh 'docker build -t cicd-demo .'
            }
        }

        stage('Deploy') {
            steps {
                sh 'echo "Push to Render via GitHub"'
            }
        }
    }
}