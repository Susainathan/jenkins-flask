pipeline {
    agent any
    environment {
        DOCKERHUB_CREDENTIALS = credentials('Docker-Hub')
        }
    stages {
        stage('Build') { 
            steps {
                echo "This is Build stage."
            }
        }
        stage('Test') { 
            steps {
                echo "This is Test stage." 
            }
        }
        stage('Deploy') { 
            steps {
                echo "This is Deploy stage." 
            }
        }
    }
}
