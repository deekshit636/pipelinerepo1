pipeline {
    agent any
parameters {
  file '/home/ubuntu/dir1'
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
