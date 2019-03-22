pipeline {
  agent any
  stages {
    stage('IBM-DNG') {
      steps {
        echo 'DNG Stage'
      }
    }
    stage('IBMRRTC') {
      steps {
        echo 'IBMRRTC stage'
      }
    }
    stage('ModelAdvisor') {
      steps {
        echo 'ModelAdvisor Step'
      }
    }
    stage('Gerrit-Code') {
      steps {
        echo 'Gerrit-Code Step'
      }
    }
    stage('QAC') {
      parallel {
        stage('QAC') {
          steps {
            echo 'QAC Parallel Step'
          }
        }
        stage('Polyspace') {
          steps {
            echo 'Polyspace parallel step'
          }
        }
        stage('LDRA') {
          steps {
            echo 'LDRA parallel step'
          }
        }
      }
    }
    stage('MatlabSimuLinkTest') {
      steps {
        echo 'MatlabSimuLinkTest Step'
      }
    }
    stage('CantataTest') {
      steps {
        echo 'Cantata Step'
      }
    }
    stage('ECUTest') {
      steps {
        echo 'ECUTest step'
      }
    }
  }
}