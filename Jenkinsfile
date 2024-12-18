pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'Runnning build automation'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
