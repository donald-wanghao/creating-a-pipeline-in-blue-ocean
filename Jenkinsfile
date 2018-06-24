pipeline {
  agent {
    node {
      label 'master'
    }

  }
  stages {
    stage('Build') {
      steps {
        bat 'npm install'
      }
    }
    stage('Test') {
      agent {
        node {
          label 'master'
        }

      }
      steps {
        bat 'echo "test stage"'
      }
    }
  }
}
