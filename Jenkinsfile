pipeline {
  agent any
  stages {
    stage('checkout stage') {
      steps {
        sh 'rm -rf GrafanaRepo'
        sh 'git clone https://github.com/Jagruthi111/GrafanaRepo.git'
      }
    }
    stage('running playbook') {
      steps {
        sh 'ansible-playbook -i hosts grafdemo.yml'
      }
    }
  }
}
