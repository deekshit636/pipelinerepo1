pipeline {
    agent any
parameters {
  password defaultValue: '123', name: 'myPassvar'
}

    stages {
        stage('Build') {
            steps {
                echo 'Building...'
            }
        }
        stage('Approval') {
            steps {
                echo 'Approval stage'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying to production...'
            }
        }
    }
}
