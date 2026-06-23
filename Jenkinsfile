pipeline {
    agent any

    stages {

        stage('Clone') {
            steps {
                git branch: 'main', url: 'https://github.com/pshusale/my-demo-app.git'
            }
        }

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t my-demo-app:v1 .'
            }
        }

        stage('Deploy Container') {
            steps {
                sh '''
                docker stop my-demo-container || true
                docker rm my-demo-container || true
                docker run -d -p 8081:80 --name my-demo-container my-demo-app:v1
                '''
            }
        }
    }
}
