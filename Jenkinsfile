pipeline {
  agent any
  stages {
    stage('Initialize') {
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