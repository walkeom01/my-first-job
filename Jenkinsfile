pipeline {
    agent any
    enviroment {
        APP_ENV = 'test'
    }
    stages {
      stage('Checkout') {
        steps {
          checkout scm 
        }
      }
      stage('Build') {
        steps {
          sh 'echo Running tests'
        }
      }
    }
    post {
      success {
          echo 'all stages passed'
      }
      failure {
          echo 'something failed'
      }
    }  
