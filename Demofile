pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                echo 'Fetching code from repo'
            }
        }

        stage('Build') {
            steps {
                echo 'Building application'
            }
        }

        stage('Services') {
            failFast false
            parallel {

                stage('PythonService') {
                    steps {
                        echo 'Building Python Service'
                    }
                }

                stage('AnalyticsService') {
                    steps {
                        echo 'Building Analytics Service'
                    }
                }

                stage('UIService') {
                    steps {
                        echo 'Building UI Service'
                    }
                }

            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application'
            }
        }

    }
}
