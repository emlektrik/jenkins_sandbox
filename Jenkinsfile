pipeline {
  agent {
    node {
      label 'linux_agents'
    }

  }
  stages {
    stage('set up env') {
      steps {
        script {
          def test_var = "haha"
        }

        ws(dir: 'scm') {
          git(url: 'https://github.com/emlektrik/jenkins_sandbox.git', branch: 'jenkins_sandbox')
          sh '''ls -lah;
echo "${test_var}";'''
        }

      }
    }

  }
}