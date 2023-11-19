pipeline {
  agent {
    node {
      label 'linux_agents'
    }

  }
  stages {
    stage('set up env') {
      steps {
        ws(dir: 'scm') {
          sh 'gcc ./main.c'
        }

      }
    }

  }
}