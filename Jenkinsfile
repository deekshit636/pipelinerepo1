pipeline {
    agent any
parameters {
  run filter: 'ALL', name: 'runParam2', projectName: 'pipelinejob1'
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
