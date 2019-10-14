pipeline{
 agent any {
  stage('repository')
        {
        echo 'running gradle scripts'
        sh './gradlew build --no-daemon'
        
         }
    stage('artifact')
    {
    archiveArtifacts 'dist/trainSchedule.zip'
    }
   }
}
