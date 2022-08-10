pipeline
{
 agent any
  stages
  {
    stage("run frontend...")
    {
      steps
      {
        echo 'executing yarn...'
        nodejs('myNodeJs')
       {
        sh 'yarn install'
        echo 'with yarn...'
       }
      }
    }
    stage("run backend")
    {
      steps
      {
         echo 'executing gradle...'
         withGradle() {
         chmod +x gradlew
         sh './gradlew -v'
         }
      }
    }
  }
}
node
{
  //grovy script
}
