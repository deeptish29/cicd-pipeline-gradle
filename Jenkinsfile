pipeline {
 agent any
 stages {
  stage('build') {
    steps {
      echo 'Running build Automation'
      sh './gradlew build --no-daemon'
      archiveArtifacts artifacts: 'dist/sampleapp.zip'
     }
    }
   }
 }
