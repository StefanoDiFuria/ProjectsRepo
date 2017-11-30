pipeline {
  agent any
  stages {
    stage('Checkout') {
      steps {
        git(url: 'https://github.com/StefanoDiFuria/ProjectsRepo.git', branch: 'develop')
      }
    }
    stage('Build') {
      steps {
        sh 'cd gs-maven;mvn clean install;'
      }
    }
  }
}