pipeline {
  agent {
    docker {
      image 'bigtruedata/sbt'
    }
    
  }
  stages {
    stage('Build') {
      steps {
        node(label: 'docker') {
          sh 'sbt build'
        }
        
      }
    }
  }
}
