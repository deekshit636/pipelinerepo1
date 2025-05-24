pipeline {
    agent any

    environment {
        PROJECT_DIR = 'c-project'
        BINARY_NAME = 'ABC.exe'
    }

    stages {
        stage('Checkout Pipeline Repo') {
            steps {
                echo 'Using Jenkinsfile from pipelinerepo1'
                // This is done automatically in a multibranch pipeline or Git trigger
            }
        }

        stage('Clone C Project Repo') {
            steps {
                sh '''
                    rm -rf ${PROJECT_DIR}
                    git clone -b main https://github.com/deekshit636/c-proj-repo.git ${PROJECT_DIR}
                '''
            }
        }

        stage('Build with Makefile') {
            steps {
                dir("${PROJECT_DIR}") {
                    sh 'make'
                }
            }
        }

        stage('Run Binary') {
            steps {
                dir("${PROJECT_DIR}") {
                    sh './${BINARY_NAME} || echo "${BINARY_NAME} exited with non-zero status"'
                }
            }
        }
    }

    post {
        success {
            echo 'Pipeline completed successfully!'
        }
        failure {
            echo 'Pipeline failed. Check logs.'
        }
    }
}
