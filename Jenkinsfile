pipeline {
    agent any
 parameters {
  choice choices: ['apple', 'banana'], name: 'MychoicePara'
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
