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
        withGradle()
       {
        sh chmod +x gradlew
        sh './gradlew -v'
        echo 'with gradle...'
       }
      }
    }
  }
}
node
{
  //grovy script
}
