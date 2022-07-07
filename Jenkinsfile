pipeline {
  agent any
  stages {
    stage('git') {
      steps {
        git 'https://github.com/kishorekk12/webAppExample.git'
      }
    }

    stage('') {
      steps {
        sh 'mvn install'
      }
    }

    stage('deploy') {
      steps {
        sh 'mvn deploy'
      }
    }

  }
}