pipeline {
  agent {
    node {
      label 'linux_agents'
    }

  }
  stages {
    stage('prepare env') {
      steps {
        ws(dir: 'scm') {
          git(url: 'https://github.com/emlektrik/jenkins_sandbox.git', branch: 'jenkins_sandbox')
          sh '''ls -lah;
echo ${workspace}'''
        }

      }
    }

  }
}