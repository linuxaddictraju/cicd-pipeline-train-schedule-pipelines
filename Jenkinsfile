pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'Running Build Automation'
        sh './gradlew build --no-daemon'
        echo "This is edited"
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
