pipeline {
 agent any
 stages {
  stage('Checkout'){
   checkout scm
   }
  stage('Build') {
    steps {
      echo 'Running build Automation'
      sh './gradlew build --no-daemon'
      archiveArtifacts artifacts: 'dist/sampleapp.zip'
     }
    }
   }
 }
