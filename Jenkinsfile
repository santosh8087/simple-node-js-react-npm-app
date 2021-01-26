pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                bat "npm install"
                bat "npm run build"
            }
        }
        stage('Test') {
                    steps {
                        bat 'npm run test'
                    }
                }
        stage('Deliver') {
                       steps {
                               sh 'npm run start'
                            }
                        }

    }
}
