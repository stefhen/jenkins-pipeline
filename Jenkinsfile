pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
       checkout([$class: 'GitSCM', branches: [[name: '*/master']], userRemoteConfigs: [[url: 'https://github.com/nmap/nmap.git']]])
       sh './configure && make'
      }
    }
    stage('Artifacts') {
      archiveArtifacts artifacts: '**/nmap', fingerprint: true
    }
  }
}
