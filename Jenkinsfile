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
       }
      }
    }
    stage("run backend")
    {
      steps
      {
        echo 'executing gradle...'
        withGradle()
       {
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
