pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
       checkout([$class: 'GitSCM', branches: [[name: '*/master']], userRemoteConfigs: [[url: 'https://github.com/nmap/nmap.git']]])
      }
    }
  }
}
