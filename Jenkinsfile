pipeline {
  agent any
  options {
    buildDiscarder(logRotator(numToKeepStr: '5'))
  }
  environment {
    DOCKERHUB_CREDENTIALS = credentials('Docker-Hub')
  }
  stages {
    stage('Login') {
      steps {
        sh 'echo $DOCKERHUB_CREDENTIALS_PSW | docker login -u $DOCKERHUB_CREDENTIALS_USR -p $DOCKERHUB_CREDENTIALS_PSW'
      }
    }
    stage('Pull') {
      steps {
        sh 'docker pull susainathan253253/jenkins_project_flask-app:latest'
        echo "Pulled docker image"
      }
    }
  }
  post {
    always {
      sh 'docker logout'
    }
  }
}
