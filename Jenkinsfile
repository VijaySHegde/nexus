@Library('shlib')_
pipeline{
  agent any
  stages{
stage("confluenceConnector"){
            steps{
           confluenceConnectorSpace()
              confluenceLogs('space created')
            }
              post{
                failure
                {
                  confluenceLogs('failed to create space')
        }
        }
            }
stage("confluenceCollector")
    {
      steps{
        confluenceCollectorSpace()
          confluenceLogs1('collected space info')
      }
      post{
        failure
        {
          confluenceLogs1('coudnt collect info')
        }
  }
    
    
  }
  }


}


