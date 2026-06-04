pipeline {
    agent any

    stages {

        stage('Docker Build') {
            steps {
                bat 'docker build -t paarth300/node-app:v1 .'
            }
        }

        stage('Docker Login') {
            steps {
                withCredentials([usernamePassword(
                    credentialsId: 'dockerhub-creds',
                    usernameVariable: 'DOCKER_USER',
                    passwordVariable: 'DOCKER_PASS'
                )]) {
                    bat 'docker login -u %DOCKER_USER% -p %DOCKER_PASS%'
                }
            }
        }

        stage('Docker Push') {
            steps {
                bat 'docker push paarth300/node-app:v1'
            }
        }
    }
}