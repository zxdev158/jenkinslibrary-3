#!groovy
@Library('jenkinslibrary@master') _

def nexus = new org.devops.nexus()

pipeline{
  agent{
    node {label "master"}
    }
  stages{
    stage("UpdateArtifact"){
      steps{
        script{
          nexus.ArtifactUpdate(updateType,artifactUrl)
        }
      }
    }
  }
}
