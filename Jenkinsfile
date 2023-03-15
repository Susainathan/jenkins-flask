pipeline {
  agent any
  stages {
    stage('Test') {
      steps {
        echo "Test run"
      }
    }
    stage('build') {
      steps {
        sh "docker-compose build"
      }
    }
  }
}
