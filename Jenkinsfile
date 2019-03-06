pipeline {
  agent any
  stages {
    stage('Integrate') {
      parallel {
        stage('Integrate') {
          steps {
            git 'https://github.com/moritzlauper/TestJenkins.git'
          }
        }
        stage('Test 1 Stage') {
          steps {
            echo 'test 1'
          }
        }
        stage('Test 2 Stage') {
          steps {
            echo 'test 2'
          }
        }
      }
    }
    stage('Test') {
      steps {
        echo 'worked'
      }
    }
  }
}