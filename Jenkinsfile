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
          script {
            test_var = "haha"
          }

          git(url: 'https://github.com/emlektrik/jenkins_sandbox.git', branch: 'jenkins_sandbox', credentialsId: '1250bd34-b292-455f-8508-2aff529cd8f0')
          sh 'gcc ./main.c'
        }

      }
    }

  }
}