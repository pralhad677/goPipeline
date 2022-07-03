pipeline {
  agent any
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
