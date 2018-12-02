pipeline {
  agent {
    docker {
      image 'maven'
    }

  }
  stages {
    stage('package') {
      steps {
        readMavenPom(file: 'pom.xml')
      }
    }
  }
}