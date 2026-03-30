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
                sh 'echo "Running tests..."'
            }
        }

        stage('Deploy') {
            steps {
                sh 'docker run -d -p 10000:10000 cicd-demo'
            }
        }
    }
}