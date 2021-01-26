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
                       echo "test done"
                    }
                }
        stage('Deliver') {
                       steps {
                               bat 'npm run start'
                            }
                        }

    }
}
