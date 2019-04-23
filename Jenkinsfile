pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'Build step'
      }
    }
    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'Test step'
          }
        }
        stage('Opencv') {
          steps {
            echo 'This is open cv'
          }
        }
        stage('Hardware') {
          steps {
            echo 'This is hardware'
          }
        }
        stage('Compiler') {
          steps {
            echo 'This is compiler stage'
          }
        }
      }
    }
    stage('Deploy') {
      steps {
        echo 'This is deploy phase'
      }
    }
  }
}