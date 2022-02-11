pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'docker build -t docker-getting-started .'
            }
        }
        stage('Test') {
            steps {
                sh 'docker run -dp 3002:3000 docker-getting-started'
            }
        }
    }
}
