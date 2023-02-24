pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'g++ -o sunidhi PES1UG20CS707.cpp'
        build job : 'PES1UG20CS707-1'
        echo 'Build stage successful'
      }
    }
    stage('Test') {
      steps {
        sh './xyz'
        echo 'Test stage successful'
      }
    }
    stage('Deploy') {
      steps {
        sh 'echo "Deploying"'
        echo 'Deployment successful'
      }
    }
  }
  post {
    failure {
      echo 'Pipeline failed'
    }
  }
}
