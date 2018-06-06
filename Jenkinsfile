pipeline {
  agent {
    dockerfile {
      filename 'Dockerfile'
    }

  }
  stages {
    stage('Dockerbuild') {
      steps {
        git 'https://github.com/jwkidd3/thedock'
      }
    }
    stage('error') {
      steps {
        sh 'sudo docker build -t=jkidd/web .'
      }
    }
  }
}