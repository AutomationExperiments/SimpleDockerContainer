pipeline {
  agent any
  stages {
    stage('Start Docker') {
      steps {
        echo '"Starting a Docker pipeline"'
        pwd()
      }
    }
    stage('Pull From Repo') {
      steps {
        git(branch: 'master', changelog: true, url: 'https://github.com/BurritoBear/SimpleDockerContainer.git')
      }
    }
  }
}