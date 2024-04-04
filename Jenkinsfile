pipeline {
  agent any
  stages {
    stage('check out') {
      steps {
        git(url: 'https://github.com/LeocFTW/jenkins_practice.git', branch: 'master')
      }
    }

    stage('run') {
      steps {
        sh 'mvn verify'
      }
    }

    stage('added steps') {
      steps {
        sh '''mvn test
mvn verify
mvn clean'''
      }
    }

  }
  tools {
    maven 'mvn_3.9.6'
    jdk 'jdk-8'
  }
}