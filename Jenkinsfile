//Map modules = [:]
@Library('shlib')_
pipeline{
  agent any
  stages{
/*stage("confluenceConnector"){
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
          confluenceLogs('collected space info')
      }
      post{
        failure
        {
          confluenceLogs('coudnt collect info')
        }
  }
    
    
  }
  */
   /* stage("confluenceContent")
    {
      steps{
        confluenceContent()
      }
    } */
  /*  stage("confluenceDelte")
    {
      steps{
        confluenceDeleteSpace()
      }
    } */
    
  /*  stage("space crreation")
    {
      steps{
        confluenceConnectorSpaceJ(jsondata)
      }
    } */
   /* stage("content creation")
    {
      steps{
        confluenceContentJ(jsondata)
      }
    } */
   /* stage("private space creation")
    {
      steps{
        confluencePrivateSpaceJ(jsondata)
      }
    } */
   /* stage("collectorspace")
    {
      steps{
        confluenceCollectorSpaceJ(jsondata)
      }
    } */
  /*  stage("collectorspace")
    {
      steps{
        confluenceGetGroupJ(jsondata)
      }
    } */
   stage("get group")
    {
      steps{
        confluenceGroupJ(jsondata)
      }
    } 
 /*   stage("get group members")
    {
      steps{
        confluenceGroupMemberJ(jsondata)
      }
    } */
   /* stage("GetSpaceInfo")
    {
      steps{
        confluenceCollectorSpaceJ(jsondata)
      }
  }*/
    
    
 /*   stage("delete page")
    {
      steps{
        confluenceDeleteContentJ(jsondata)
      }
  }
  */
  /*  stage("testing")
    {
      steps
      { script{
        confluenceTest.call(jsondata)
      }
    }
    }
    
     stage("grouping")
    {
      steps
      { script{
        confluenceTest.info(jsondata)
      }
    }
    }
    
  /*  stage("getgroup")
    {
      steps{
        script
        {
        log.call(jsondata)
      }
  }
    }
    */
    
    
  }

}


