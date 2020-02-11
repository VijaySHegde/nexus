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
    
  /*stage("space_creation")
    {
      steps{
        confluenceConnectorSpaceJ(jsondata)
      }
    } 
   stage("private space creation")
    {
      steps{
        confluencePrivateSpaceJ(jsondata)
      }
    } 
    stage("content creation")
    {
      steps{
        confluenceContentJ(jsondata)
      }
    } 
    
    stage("collectspace")
    {
      steps{
        confluenceCollectorSpaceJ(jsondata)
      }
    } 
    
    stage("getAllgroups")
    {
      steps{
        confluenceGetGroupJ(jsondata)
       
      }
    } 
    
  stage("getAgroup")
    {
      steps{
        confluenceGroupJ(jsondata)
      }
    } 
    stage("getGroupMember")
    {
      steps{
        confluenceGroupMemberJ(jsondata)
      }
    } 
    
   
   /* stage("GetSpaceInfo")
    {
      steps{
        confluenceCollectorSpaceJ(jsondata)
      }
  }*/
    
    
 /* stage("delete page")
    {
      steps{
        confluenceDeleteContentJ(jsondata)
      }
  }
  
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
    stage("page count")
    {
      steps{
        script {
        def responeJson = confluence_collector()
        println(responeJson)
        }
      }
  }
  
    
   /* stage("page")
    {
      steps{
        confluenceCollectorSpaceJ()
      }
    }*/
  }

}


