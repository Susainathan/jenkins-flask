pipeline {
  agent any
  options {
    buildDiscarder(logRotator(numToKeepStr: '5'))
  }
  environment {
    DOCKERHUB_CREDENTIALS = credentials('Docker-Hub')
  }
  stages {
    stage('Build') {
      steps {
        sh 'docker-compose build'
      }
    }
    stage('Test') {
      steps {
        echo "Test run
      }
    }
  }
  post {
    always {
      sh 'docker logout'
    }
  }
}
