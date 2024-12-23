pipeline {
  node any
  stages {
    stage ('Build') {
      step {
        echo 'Running build automation...'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
