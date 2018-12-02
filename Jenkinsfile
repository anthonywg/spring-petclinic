pipeline {
  agent {
    docker {
      image 'debiab'
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
    stage('') {
      steps {
        sh './mvnw clean package'
      }
    }
  }
}