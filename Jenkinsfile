pipeline {
  agent {
    docker {
      image 'docker pull bigtruedata/sbt'
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