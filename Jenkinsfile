pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/aryakajal1002-cell/CI_Pipeline.git'
            }
        }

        stage('Build') {
            steps {
                echo 'Building project from GitHub...'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application...'
            }
        }
    }
}
