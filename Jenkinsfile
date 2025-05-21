pipeline {
    agent any
parameters {
  text defaultValue: 'value hhere', name: 'textPara1'
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
