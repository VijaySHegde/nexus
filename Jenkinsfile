 stage('Mvn Package'){
     def mvnHome = tool name: 'maven-3', type: 'maven'
     def mvnCMD = "${mvnHome}/bin/mvn"
     sh "${mvnCMD} clean package"
   }
   stage('Build Docker Image'){
     sh 'docker build -t kammana/my-app:2.0.0 .'
   }
   stage('Push Docker Image'){
     withCredentials([string(credentialsId: 'docker-pwd', variable: 'dockerHubPwd')]) {
        sh "docker login -u kammana -p ${dockerHubPwd}"
     }
     sh 'docker push kammana/my-app:2.0.0'
   }
   stage('Run Container on Dev Server'){
     def dockerRun = 'docker run -p 8080:8080 -d --name my-app kammana/my-app:2.0.0'
     sshagent(['dev-server']) {
       sh "ssh -o StrictHostKeyChecking=no ec2-user@172.31.18.198 ${dockerRun}"
     }
   }
}

/*

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
   /* stage("page count")
    {
      steps{
        script {
        def responseJson = confluence_collector.call()
          println (responseJson)
          echo responseJson
          //println(responseJson.totalSize)
        }
      }
  }
  */
    
    
    stage("page")
    {
      steps{
        
          
        confluenceCollectorSpaceJ(jsondata)
        influxDb()
        }
      
    }
  }

}


*/
