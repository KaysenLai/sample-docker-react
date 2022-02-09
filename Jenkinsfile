pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'sudo su -'
                sh 'docker build -t docker-getting-started .'
            }
        }
        stage('Test') {
            steps {
                sh 'docker run -dp 3000:3000 docker-getting-started'
            }
        }
    }
}