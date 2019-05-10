pipeline {
  agent {
    docker {
      image 'mysql'
    }

  }
  stages {
    stage('step1') {
      agent {
        dockerfile {
          filename 'mysql'
        }

      }
      steps {
        dockerNode(image: 'mysql') {
          sleep 3
        }

      }
    }
  }
}