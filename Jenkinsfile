pipeline {
  agent any
  stages {
    stage('check out') {
      steps {
        sh 'git(url: \'https://github.com/LeocFTW/jenkins_practice.git\', branch: \'master\')'
      }
    }

  }
  environment {
    maven = 'mvn'
  }
}