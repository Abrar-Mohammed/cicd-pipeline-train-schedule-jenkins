pipeline{
  agent any
  stages{
    
    stages('build') {
      steps{
        echo 'Running the build automation'
        sh './gradlew build --no-deamon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
