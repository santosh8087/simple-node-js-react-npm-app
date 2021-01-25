pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh "npm install"
                sh "npm run build"
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
