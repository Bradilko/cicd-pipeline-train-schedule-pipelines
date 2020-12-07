pipeline {
  agent any
  stages {
    stage ("build") {
      steps {
        echo 'Running build automation'
        sh './gradle build" --no=-daemon'
        archiveArtifacts artifact: 'dist.trainSchedule.zip'
      }
    }
  }
}
