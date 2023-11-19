pipeline {
  agent {
    node {
      label 'linux_agents'
    }

  }
  stages {
    stage('run c') {
      steps {
        sh 'ls; gcc ./main.c;'
      }
    }

  }
}