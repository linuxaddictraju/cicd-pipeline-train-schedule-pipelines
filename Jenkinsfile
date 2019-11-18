pipeline {
  agent any
  stages ('Build') {
    steps {
      echo 'Running Build Automation'
      sh './gradlew build --no-daemon'
      archiveArtifacts artifacts: 'dist/trainSchedule.zip'
    }
  }
}
