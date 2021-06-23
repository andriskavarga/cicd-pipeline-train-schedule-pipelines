pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh './gradlew build --no-daemon'
      }
    }
    stage('Archive') {
      steps {
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
