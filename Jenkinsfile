pipeline {
  agent {
    node {
      label 'linux_agents'
    }

  }
  triggers { cron('H */5 * * * * ') }
  stages {
    stage('run c') {
      steps {
        sh 'ls; gcc ./main.c;'
        sshagent(credentials: ['1250bd34-b292-455f-8508-2aff529cd8f0']) {
      sh '''
        echo haha;
      '''
    }
      }
    }

  }
}
