@Library('shlib')_
pipeline{
 agent any
   tools{
        maven "Maven"
    }

  stages{
stage("c"){
            steps{
           confluenceConnectorSpace()
              confluenceLogs('space created')
            }
             
            }
}
}
