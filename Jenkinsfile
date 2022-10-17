pipeline {
  agent any
  tools {
  maven 'mvn'
  }
  
  stages {
    stage ('Hello') {
      steps {
              git 'https://github.com/yashaswini-ltts/sample.git'
            }
         }
    stage ('Compile') {
      steps {
            echo 'mvn clean package'
      }
    }
    stage ('deployment') {
      steps {
            echo 'mvn deploy'
      }
    }
    stage ('docker') {
      steps {
            echo 'mvn docker'
      }
    }
  }
}
    
