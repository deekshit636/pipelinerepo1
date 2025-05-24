pipeline {
    agent any

    environment {
        BINARY_NAME = "ABC.exe"
    }

    stages {
        stage('Clone Repository') {
            steps {
                git url: 'https://github.com/deekshit636/c-proj-repo.git'
            }
        }

        stage('Build with Makefile') {
            steps {
                sh 'make'
            }
        }

        stage('Run Binary') {
            steps {
                sh './${BINARY_NAME} || echo "${BINARY_NAME} exited with non-zero status"'
            }
        }
    }

    post {
        success {
            echo 'Build and execution completed successfully!'
        }
        failure {
            echo 'Build or execution failed. Check console output.'
        }
    }
}
pipeline {
    agent any

    environment {
        BINARY_NAME = "ABC.exe"
    }

    stages {
        stage('Clone Repository') {
            steps {
                git url: 'https://github.com/deekshit636/c-proj-repo.git'
            }
        }

        stage('Build with Makefile') {
            steps {
                sh 'make'
            }
        }

        stage('Run Binary') {
            steps {
                sh './${BINARY_NAME} || echo "${BINARY_NAME} exited with non-zero status"'
            }
        }
    }

    post {
        success {
            echo 'Build and execution completed successfully!'
        }
        failure {
            echo 'Build or execution failed. Check console output.'
        }
    }
}
