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
        sh sudo apt-get install gradle
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
