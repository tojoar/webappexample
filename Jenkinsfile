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
        deploy adapters: [tomcat8(credentialsId: '9c41f7f4-5a9d-4f72-8a3f-142d322f46e9', path: '', url: 'http://localhost:8081/')], contextPath: null, war: '*/*.war'
      }
    }

  }
}
