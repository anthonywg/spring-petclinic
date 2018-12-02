pipeline {
  agent {
    docker {
      image 'debian'
    }

  }
  stages {
    stage('package') {
      agent {
        docker {
          image 'debian'
        }

      }
      steps {
        sh 'mvn clean package'
      }
    }
  }
}