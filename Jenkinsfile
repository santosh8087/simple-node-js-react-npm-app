pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                bat 'npm install'
                bat 'npm run build'
            }
        }
        stage('Test') {
                    steps {
                        bat 'npm run test'
                    }
                }
        stage('Deliver') {
                       steps {
                                bat './jenkins/scripts/deliver.sh'
                                input message: 'Finished using the web site? (Click "Proceed" to continue)'
                                bat './jenkins/scripts/kill.sh'
                            }
                        }

    }
}
