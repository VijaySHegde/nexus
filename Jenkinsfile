@Library('shlib')_
pipeline{
  agent any
  stages{
stage("confluence"){
            steps{
           confluenceConnectorSpace()
              confluenceLogs('success')
              post{
                failure
                {
                  confluenceLogs('failed')
        }
        }
    )
  }
}
