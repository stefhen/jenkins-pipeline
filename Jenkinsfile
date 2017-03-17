pipeline {
  agent any
    stages {
      stage('Build') {
        steps {
          git url: 'https://github.com/nmap/nmap.git'
          sh './configure && make'
          archiveArtifacts artifacts: '**/nmap', fingerprint: true
       }
     }
   }
   post {
     always {
       sh 'make test'
     }
   }
 }
