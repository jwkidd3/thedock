pipeline {
  agent none
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