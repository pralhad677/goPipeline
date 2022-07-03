pipeline {
  agent any
  stages {
    stage('build') {
      steps {
         
      echo ${name} 
        sudo chmod +x a.go
        go run a.go
      }
    }

  }
  environment {
    name = 'jacob'
  }
}
