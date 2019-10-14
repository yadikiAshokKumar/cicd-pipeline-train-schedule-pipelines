pipeline{
 agent any
 stages {
  stage('repository')
        {
         
         steps{
        echo 'running gradle scripts'
        sh './gradlew build --no-daemon'
         }
         }
    stage('artifact')
    {
     steps{
    archiveArtifacts 'dist/trainSchedule.zip'
    }
    }
   }
}
