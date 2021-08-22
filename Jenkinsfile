pipeline {
 agent any
 stages {
  stage('Git') {
   steps {git 'https://github.com/dmitry-izjurov/netology-test.git'}
  }
  stage('Test') {
   steps {
    sh 'go test .'
   }
  }
  stage('Build') {
   steps {
    sh 'docker build .'
   }
  }
 }
}
