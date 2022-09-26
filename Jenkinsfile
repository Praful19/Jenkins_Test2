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
    stage("Deploy To Dev 2.0 "){
      steps{
         sh "mvn clean deploy"
      }
    }
    stage("Deploy To Test 2.0 "){
      steps{
         echo "Test is success"
      }
    }
  }
}
