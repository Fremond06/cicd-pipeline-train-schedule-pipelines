pipeline {
  agent any
  stages {
    stage ('Build') {
      step {
        echo 'Running build automation'
        sh './gradlew build --no-daemon'
        archineArtifacts artifacts: 'dist/tranSchedule.zip'
      }
    }
  }
}
