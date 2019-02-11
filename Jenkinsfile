pipeline {
  agent any {
    stages ('build') {
      steps {
        echo 'Running build automation'
        sh './gradlew.sh build --no-daemon'
        archiveArtifact artifact: 'dist/trainSchedule.zip'
      }
    }
  }
}
