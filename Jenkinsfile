pipeline {
  agent any
  stages {
    stage('Build Application') { 
      steps {
        bat 'mvn clean install'
      }
    }
    stage('Deploy Mule Application into cloud') { 
      steps {
        bat 'mvn clean package deploy -DmuleDeploy'
      }
    }
}
}