pipeline {
  agent {
    node {
      label 'linux_agents'
    }

  }
  stages {
    stage('set up env') {
      String test_var='test var'
      steps {
        ws(dir: 'scm') {
          git(url: 'https://github.com/emlektrik/jenkins_sandbox.git', branch: 'jenkins_sandbox')
          sh '''ls -lah;
echo "$test_var;"'''
        }

      }
    }

  }
}
