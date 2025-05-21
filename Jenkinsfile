pipeline {
    agent any
parameters {
  string defaultValue: '20', name: 'abc'
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
