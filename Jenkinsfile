pipeline {
  agent any
  stages {
    stage('PRE-BUILD STUFF HERE') {
      steps {
        sh 'echo STEFHEN PRE BUILD STUFF'
      }
   }
    stage('BUILD STUFF HERE') {
      steps {
        sh 'echo BUILD STUFF HERE'
      }
    }
    stage('Test') {
      steps {
        sh 'make check || true'
      }
    }
  }
}
