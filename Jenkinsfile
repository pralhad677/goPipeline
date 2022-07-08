def firstName = null
pipeline {
  agent any
  tools {
    go '1.18.3'
  }
  stages {
    stage('input'){
      agent none
      name = input(
        message:"your name please!!",
        ok:"submit",
        parameter:[string(defaultValue:"jacob",name:"Name",trim:true)]
      )
    }
    stage('build') {
      steps {
        script{
 
    
             sh '''#!/bin/bash
                 echo "hello world" 
                   echo "${name}" 
                     echo "${firstName}" 
                 sudo chmod +x a.go
        go run a.go 
         '''
        
        }
      }
    }

  }
  environment {
    name = 'jacob'
  }
  post {
        always {
            echo "This block always runs."
        }
  }
}
