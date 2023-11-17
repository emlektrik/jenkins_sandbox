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

          git(url: 'https://github.com/emlektrik/jenkins_sandbox.git', branch: 'jenkins_sandbox')
          sh "echo ${test_var}"
        }

      }
    }

  }
}