pipeline {
 agent any
 stages {
  stage('checkout'){
   steps{
    sh 'git checkout -b cicd-pipeline-gradle'
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
