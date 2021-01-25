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
                        echo "test1"
                    }
                }
        stage('Deliver') {
                       steps {
                               echo "deliver"
                            }
                        }

    }
}
