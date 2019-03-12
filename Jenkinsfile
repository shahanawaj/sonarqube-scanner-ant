pipeline
{
  environment
   {
    antVersion = 'ant 1.9'
   }
  agent any

  stages
  {
    stage ('build')
    {
      steps
      {
      withEnv( ["ANT_HOME=${tool antVersion}"] ) {
      sh '$ANT_HOME/bin/ant all'
      }
}
}
/*  stage ('sonar')
  {
    steps
    {
    withEnv( ["ANT_HOME=${tool antVersion}"] ) {
    sh '$ANT_HOME/bin/ant sonar'
    }
}
}*/
}



/* post{
    always{
      archiveArtifacts '**/dist/*.*'
    }
  }*/
}
