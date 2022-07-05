pipeline {
  agent any
  tools {
    go '1.18.3'
  }
  stages {
    stage('build') {
      steps {
        script{
 
      echo "${name}" 
        sudo chmod +x a.go
        go run a.go 
        }
      }
    }

  }
  environment {
    name = 'jacob'
  }
}
