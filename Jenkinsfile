pipeline {
  agent any
  stages {
    stage('Initialize') {
      steps {
        sh 'mvn clean'
      }
    }
    stage('build') {
      steps {
        sh 'mvn install'
      }
    }
  }
}
