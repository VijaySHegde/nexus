@Library('shlib')_
pipeline{
  agent any
  stages{
stage("NexusConnector"){
            steps{
       nexusconector()
        }
        }
        stage("NexusCollector"){
            steps{
       nexuscollector()
        }
        }
}
}
