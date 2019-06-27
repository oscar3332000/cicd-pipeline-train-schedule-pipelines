pipeline {
  agent any

  stages {
    stage('build') {
      steps {
        echo 'Building project'
        sh './gradlew build --no-daemon'
        archiveArticfacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
