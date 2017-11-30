pipeline {
  agent any
  stages {
    stage('Checkout') {
      steps {
        git(url: 'git@github.com:StefanoDiFuria/ProjectsRepo.git', branch: 'develop')
      }
    }
  }
}