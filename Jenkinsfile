pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                docker login -u="$susainathansusai@gmail.com" -p="$Fleurdelis+1.618"
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
