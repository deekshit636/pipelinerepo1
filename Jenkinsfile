pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Building...'
            }
        }
        stage('Approval') {
            steps {
                input {
                    message "Do you want to deploy to production?"
                }
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying to production...'
            }
        }
    }
}
