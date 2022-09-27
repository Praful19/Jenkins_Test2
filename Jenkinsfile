@Library("mylibs") _
pipeline {
  agent any
  tools {
    maven 'maven2'
  }
  stages{
    stage("Maven Build"){
      steps{
        sh "mvn clean package"
      }
    }
    stage("Deploy To Dev 3.0 "){
      steps{
         sh "mvn clean deploy"
      }
    }
  }
}
