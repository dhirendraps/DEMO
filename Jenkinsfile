pipeline {
  agent any
  stages {
    stage('Initalize') {
      steps {
        build 'mvn clean'
      }
    }
    stage('build') {
      steps {
        build 'mvn install'
      }
    }
  }
}