pipeline {
    agent any

    stages {

        stage('Install Dependencies') {
            steps {
                bat 'npm install'
            }
        }

        stage('Build Docker Image') {
            steps {
                bat 'docker build -t paarth300/node-app:v1 .'
            }
        }

        stage('Push Docker Image') {
            steps {
                bat 'docker push paarth300/node-app:v1'
            }
        }
    }
}
