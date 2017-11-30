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
        bat 'mvn clean install -f ./gs-maven/pom.xml'
      }
    }
    stage('Sonar Analysis') {
      steps {
        bat 'mvn sonar:sonar'
      }
    }
  }
}