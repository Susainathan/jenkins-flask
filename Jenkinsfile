pipeline {
    agent any
    environment {
        DOCKERHUB_CREDENTIALS = credentials('Docker-Hubs')
        }
    stages {
        stage('Build') { 
            steps {
                echo "This is Build stage."
            }
        }
        stage('Login') {
        steps {
            sh 'echo $DOCKERHUB_CREDENTIALS_PSW | docker login -u $DOCKERHUB_CREDENTIALS_USR --password-stdin'
        }
        stage('Deploy') { 
            steps {
                echo "This is Deploy stage." 
            }
        }
    }
}
