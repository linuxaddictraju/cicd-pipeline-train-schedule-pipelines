pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'Running Build Automation'
        sh './gradlew build --no-daemon'
        sh 'mkdir example-solution'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
        sh 'cp dist/trainSchedule.zip dist/trainSchedule1.zip'
      }
    }
  }
}
