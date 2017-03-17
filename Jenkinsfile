node {
  git url: 'https://github.com/nmap/nmap.git'
  sh './configure && make'
  archiveArtifacts artifacts: '**/nmap', fingerprint: true
  sh 'aws s3 cp ${artifacts} s3://stefhen-rightscale/jenkins/'
}
