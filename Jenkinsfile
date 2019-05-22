pipeline {
  agent any
  stages {
    stage('build app') {
      steps {
        sh 'mvn install'
      }
    }
    stage('run') {
      steps {
        sh '''cd gameoflife-web/
mvn jetty:run
'''
      }
    }
  }
}