@Library('shlib')_
pipeline{
  agent any
  stages{
stage("confluence"){
            steps{
           confluenceCollectorSpace()
              confluenceLogs('success')
            }
              post{
                failure
                {
                  confluenceLogs('failed')
        }
        }
            }
  }
    
    
  }

