pipeline {
  agent {
    node {
      label 'nodeapp'
    }

  }
  stages {
    stage('Build') {
      steps {
        bat 'npm install'
        bat 'npm run build'
      }
    }

 

    stage('Deliver') {
      steps {
        bat 'npm run start'
      }
    }

  }
}
