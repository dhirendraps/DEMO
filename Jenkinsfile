pipeline {
  agent any
  stages {
    stage('Initalize') {
      steps {
        sh 'mvn clean'
      }
    }
    stage('build') {
      steps {
        build 'mvn install'
      }
    }
  }
}