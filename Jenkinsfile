pipeline {
  agent none
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
  environment {
    maven_3_6_0 = 'E:\\apache-maven-3.6.0-bin\\apache-maven-3.6.0'
    java8 = 'C:\\Program Files\\Java\\jdk1.8.0_181'
  }
}