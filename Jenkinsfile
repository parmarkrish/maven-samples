pipeline {
  agent any
  tools { 
      maven 'mvn-3.9.6' 
      jdk 'jdk-1.8' 
  }
  stages {
    stage('check out') {
      steps {
        git(url: 'https://github.com/dhetong/maven-samples-A6.git', branch: 'master')
      }
    }

    stage('run') {
      steps {
        sh 'mvn verify'
      }
    }

  }
}

