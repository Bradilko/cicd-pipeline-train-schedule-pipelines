pipeline {
  agent any
  stages {
    stage ("build") {
      steps {
        echo 'Running build automation'
        sh './gradle build" --no=-daemon'
        archiveArtifacts artifacts: 'dist.trainSchedule.zip'
      }
    }
  }
}
