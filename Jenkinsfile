pipeline {
  agent any
  
  stages {
    stage('checkout stage') {
      steps {
        sh 'rm -rf prometheus'
        sh 'git clone https://github.com/Chaitraradha/prometheus.git'
      }
    }
    stage('running playbook') {
      steps {
        sh 'ansible-playbook -i hosts prom.yml'
      }
    }
  }
}
